**Before anything else**

I created a directory on my local computer. At the same time, I made a repository online on Github. I cloned the repository onto my local directory

**Step 1**

In the original file in the datacodealongs, I ran this command in the terminal : 
cut -d’,’ -f1,2 energy_sample.csv > output.csv
I ran this same command, replacing the "2" with 3,4,5,6,7

**Columns**
Country : String, text given to label each country
Iso_code : String, text given to label each country
Year : String, although numbers, no arithmetic will be used on these values, it is used as a label.
Population : Integer, arithmetic can be done with this (max,min,avg,etc.)
Energy_per_capita : Float, number that contains decimals, and arithmetic can be done.
Fossil_share_energy : Float, number that contains decimals, and arithmetic can be done.
Renewable_share_energy : Float, number that contains decimals, and arithmetic can be done.

**How many rows and countries**

```bash
wc -l energy_sample.csv 
```

Output : 71 

The command gives me 71 rows (including the header)
Now, if we remove the header row, there are 70 rows. I looked at the data and saw each country has 7 years, 2015-2021. 70/7 will yield 10. So there are 10 countries

71 rows
10 countries


**What I found**

Both Nigeria and Kenya's data are missing from column 6 and 7 : fossil share energy and renewable share energy

I found a direct relationship between different values:
As population increases , energy per capita decreases as well

As energy per capita decreases,fossil share energy decreases as well

As fossil share energy decerases, renewables share energy increases

Just from looking at the relationship individually, we can draw a conclusion across different values as well

This means that as population increases, both energy per capita and fossil share energy decrease while renewable share energy increases.

**Step 2**

Questions my group came up with : 

Which countries along with the year had a population of over 20,000,000 and fossil share is under 90.0 

What countries had over 40 renewable share energy? 

What years after 2020 had over 100,000 energy per capita?

**Single data-quality question**

The first question my group came up with asked a direct relationship between two specific values, this got me thinking of how I can ask to compare the whole category

So I came sharpened this data-quality question:

What is the relationship between population and energy per capita, fossil share energy, and renewables share energy?
