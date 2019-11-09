# babysize
babysize compares the size and weight of an infant or toddler against the
[day-accurate standard curves of the WHO](https://www.who.int/childgrowth/standards/en/).

## Usage
Simply run the program, specifying optionally the weight, length and head
circumference of your child. Mandatory arguments are the gender and birthdate:

```
$ ./babysize -w 8.850 -l 72 -c 43 f 2019-01-01
Arm circumference for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
   11.0    11.7    12.1    12.3    12.7    13.0    13.4    14.1    15.0    15.4    15.7    16.2    16.6    17.2    18.4

Body mass index for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
   12.8    13.6    14.1    14.4    14.8    15.2    15.6    16.6    17.6    18.2    18.6    19.3    19.7    20.5    22.1
  -> Estimated 61.8% percentile for a BMI of 17.1

Head circumference for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
   40.2    41.2    41.8    42.1    42.6    42.9    43.4    44.3    45.2    45.7    46.1    46.5    46.9    47.5    48.5
  -> Estimated 16.5% percentile for a head circumference of 43 cm

Length/height for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
   64.1    66.0    67.1    67.7    68.6    69.2    70.1    71.8    73.5    74.4    75.0    75.9    76.5    77.6    79.5
  -> Estimated 52.9% percentile for a length of 72 cm

Subscapular skinfold for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
    4.0     4.5     4.8     5.0     5.3     5.5     5.9     6.6     7.6     8.1     8.5     9.2     9.7    10.7    12.8

Triceps skinfold for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
    4.4     5.2     5.6     5.9     6.3     6.7     7.2     8.2     9.4    10.2    10.7    11.5    12.1    13.3    15.7

Weight for age / Percentiles
   0.1%    1.0%    3.0%    5.0%   10.0%   15.0%   25.0%   50.0%   75.0%   85.0%   90.0%   95.0%   97.0%   99.0%   99.9%
    5.9     6.5     6.8     7.0     7.3     7.5     7.9     8.5     9.3     9.7    10.0    10.5    10.8    11.4    12.6
  -> Estimated 60.4% percentile for a weight of 8.8 kg
```

## License
Code is GNU GPL-3. All the source data contained in `who_data.json` is from the WHO.
