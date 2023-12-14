# Custom Report for Beer Smith

Requirements:
1. Ensure you have the correct costs for ingredients in your recipe.
2. Copy the recipe to a new location with a new name, possibly append it with a date `example.20231213`.
3. In the new recipe, adjust the `Batch Size` to your actual volume from kegs and cans.
4. Preview|Print the recipe and use the cog.htm report

```
Cost of Goods Report Date: Wed Dec 13 2023

Beer Name: Example Fruited Beer
Cost per Gallon: $3.40
1/6 Barrel Keg: $17.68
1/4 Barrel Keg: $26.35
1/2 Barrel Keg: $52.70
12 oz Can - Single: $0.98
12 oz Can - Case: $24.93
16 oz Can - Single: $1.09
16 oz Can - Case: $27.48
```

Adjust the cog.htm file to reflect your actual package costs. [(cog.htm)](https://github.com/cov3rt/beersmith_cog_report/blob/main/cog.htm?plain=1#L8)
```
    var packageCosts = {
        'label': 0.37,
        'can': 0.17,
        'lid': 0.05,
        'flat': 0.48,
        'packtech': 0.16,
        'shipping': 0.07
    };
```
