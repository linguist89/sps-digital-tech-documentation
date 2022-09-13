---
layout: page
title: Data Tables
navigation: 4
---

# Data Tables
Data tables have a `table_number` property to give the data table a unique id when it's added to a form. To add data to the table you need to pass in three variables: 
- `column_names` - these are going to be the names for the columns. You can add as many columns as you want, just as long as the number of column names and the data match in size.
- `table_data` - this needs to be a list of tuples. Each tuple has the same number of elements as the number of column names and they need to be in the same order to match the column names. 
- `table_number` - this finds the correct table to add the above data to it, thus needs to be passed as parameters with `column_names` and `table_data`.