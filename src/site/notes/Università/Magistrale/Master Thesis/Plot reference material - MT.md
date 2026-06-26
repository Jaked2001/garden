---
{"dg-publish":true,"permalink":"/universita/magistrale/master-thesis/plot-reference-material-mt/","tags":["MT/Support"],"dg-note-properties":{"aliases":null,"Tipo":"Documentation","Stato":null,"Parents":["[[Master Thesis]]"],"Children":null,"Siblings":null,"Cover":null,"Progetto":"[[Master Thesis]]","tags":["MT/Support"]}}
---

# [[Università/Magistrale/Master Thesis/Plot reference material - MT\|Plot reference material - MT]]


In this note, I want to include several graph templates that I use for my thesis analysis in R.

```table-of-contents
```

## Naming rules

Each plot, if potentially to be used in the dissertation, needs to:
- be stored into a **named variables** in the workplace
- called on the next line to **be shown** when the file is run,
- **saved** to a local directory.

Furthermore, each plot shall have
- **Title**
- **Labels** for x-axis and y-axis
- **Units** if appropriate
- **Style**: from ggplot: `theme_light()`
- **Legend**: show a legend if necessary to read, otherwise do not show.


## Useful snippets

### Labels

```r title:"Title and labels"
labs(
    x = "User type",
    y = "Average speed recorded [km/h]",
    title = "Speed by user type"
  ) +
```


### Axis text settings

```r title:"TITLE"
theme(axis.text.x = element_text(angle = 45, vjust = 1, hjust = 1, size = 10)) +

```

- axis.text.x: edit for x-axis
- angle: the angle of display
- vjust: vertical shift
- hjust: horizontal shift
- size: size of text of 


### Strip text settings (for faceting)

```r title:"TITLE"
theme(strip.text = element_text(size = 7, face = "bold", margin = margin(t = 2, b = 2))
```

- strip.text: edit for faceting strip text


## Plots templates

### General plot

```r
ggplot(data, aes(x = , y = , fill = , color = )) +
  
  # --- Geometries -------------------------------------------------
  geom_()+
  
  # --- Severity regions (if applicable) ---------------------------
  geom_polygon(data = Region1, aes(x = x, y = y), fill = "red",    alpha = 0.2) +
  geom_polygon(data = Region2, aes(x = x, y = y), fill = "orange", alpha = 0.2) +
  geom_polygon(data = Region3, aes(x = x, y = y), fill = "yellow", alpha = 0.2) +
  
  # --- Facets -----------------------------------------------------
  facet_wrap(~, ncol = ) +
  
  # --- Scales -----------------------------------------------------
  scale_fill_manual(name = "", values = palette_) +
  scale_color_manual(name = "", values = palette_) +
  scale_x_continuous(limits = c(, ), breaks = seq(, , by = )) +
  scale_y_continuous(limits = c(, ), breaks = seq(, , by = )) +
  # scale_x_time(date_labels = "%H:%M:%S") +  # for hms variables
  
  # --- Coordinate system ------------------------------------------
  coord_cartesian(xlim = c(, ), ylim = c(, )) +
  
  # --- Labels -----------------------------------------------------
  labs(
    x     = expression(),
    y     = expression(),
    title = "",
    fill  = "",
    color = ""
  ) +
  
  # --- Theme ------------------------------------------------------
  theme(
    axis.text.x  = element_text(angle = 45, vjust = 1, hjust = 1, size = ),
    axis.text.y  = element_text(size = ),
    strip.text   = element_text(size = , face = "bold", margin = margin(t = 2, b = 2)),
    legend.position = "none"  # "none", "bottom", "top", "left", "right"
  )

```

### Boxplot + Violin


```r title:"Boxplot + violin"


plotName <- ggplot(df, aes(x = df_x, y = df_y, fill = df_style)) +
  geom_violin(alpha = 0.3, show.legend = FALSE, color = NA) +
  geom_boxplot(width = 0.2, notch = FALSE,  show.legend = FALSE,  color = NA, outlier.size = 0.25, outlier.color = "black") +
  # For single plot, comment out next line
  facet_wrap(~df_facet) +
  labs(
    x = "User type",
    y = "Average speed recorded [km/h]",
    title = "Speed by user type"
  ) +
  theme(axis.text.x = element_text(angle = 45, vjust = 1, hjust = 1, size = 10), 
        strip.text = element_text(size = 7, face = "bold", margin = margin(t = 2, b = 2))
        )+
  scale_fill_manual(values = palette_colors) # for custom colors 

Speed_by_user_boxplot # Show plot
save_plot(Speed_by_user_boxplot, "SpeedByUser.pdf") # Save plot

```

```r title:"TITLE"
conflictRatePer1000users_dir_PETseverity_plot <- ggplot(conflictRate_perDir_long_PETseverity |> filter(Obj == "Obj1"), # Filter because it's in long form
       aes(x = PET_Severity,
           y = Direction,
           fill = conflRateCum)) +
  geom_tile(color = "white") +
  geom_text(aes(label = round(conflRateCum,1)),
            color = "black", size = 4) +
  facet_wrap(~Intersection) +
  scale_fill_gradient(low = "#deebf7", high = "#3182bd",limits = c(0, 400)) +
  #theme_minimal(base_size = 12) +
  theme(
    axis.text.x = element_text(angle = 0, hjust = 0.5, size=12),
    axis.text.y = element_text(angle = 0, size=12),
    panel.grid = element_blank(),
    strip.text = element_text(face = "bold"),
    legend.position = "bottom"
  ) +
  labs(
    title = "Conflicts per 1000 users in a specific direction",
    x = "PET severity",
    y = "Direction",
    fill = "Conflicts per 1000 users"
  )
```
