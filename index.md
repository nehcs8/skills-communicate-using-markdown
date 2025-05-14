# Big ass header
## one of
### header of moderate dimensions 
#### each
##### dimensions
###### im just vibin here following instructions


![Image of whatever](https://octodex.github.com/images/yaktocat.png)

``` python
def main():
    # Step 0: Load data and ask for year
    try:
        ds = xr.open_dataset('C:\Users\23chen\Documents\subset_180.nc')
    except FileNotFoundError:
        raise FileNotFoundError("File 'subset.nc' not found.")

    year = int(input("Enter year to analyze (e.g., 2005): "))
    ds_year = ds.sel(time=str(year))

    if len(ds_year.time) == 0:
        raise ValueError(f"No data for year {year}.")
```
