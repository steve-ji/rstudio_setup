# rstudio_setup
Some reminders for things I commonly use in RStudio

## Style Guide
### `select()`
When selecting columns, column names are generally unchanged, while the order of columns is much more adjustable due to `mutate()`. To prevent the manual counting of columns later on, select all your columns by name. This has an additional benefit of being more readable.
#### Bad Example
```
df = df0 %>%
  select(1:9, 11, 13)
```
#### Good Example
```
df = df0 %>%
  select(ticket_id,
         ticket_name,
         ...)
```
