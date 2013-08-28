Start working with how we might pair crossfilter and dc.js, separately or in combination, to work with R data.  Some good links are the [dc.js Nasdaq example]() and this [AAII stock picking analysis](http://www.acrodatics.com/) by [Lon Riesberg](https://twitter.com/lonriesberg).

<script>
var data =
   [
 {
 "date":   9526,
"manager": "HAM1",
"perf": 0.0074,
"cumul": 1.0074 
},
{
 "date":   9555,
"manager": "HAM1",
"perf": 0.0193,
"cumul": 1.0268 
},
{
 "date":   9586,
"manager": "HAM1",
"perf": 0.0155,
"cumul": 1.0428 
},
{
 "date":   9616,
"manager": "HAM1",
"perf": -0.0091,
"cumul": 1.0333 
},
{
 "date":   9647,
"manager": "HAM1",
"perf": 0.0076,
"cumul": 1.0411 
},
{
 "date":   9677,
"manager": "HAM1",
"perf": -0.0039,
"cumul": 1.0371 
},
{
 "date":   9708,
"manager": "HAM1",
"perf": -0.0231,
"cumul": 1.0131 
},
{
 "date":   9739,
"manager": "HAM1",
"perf": 0.0395,
"cumul": 1.0531 
},
{
 "date":   9769,
"manager": "HAM1",
"perf": 0.0147,
"cumul": 1.0686 
},
{
 "date":   9800,
"manager": "HAM1",
"perf": 0.0288,
"cumul": 1.0994 
},
{
 "date":   9830,
"manager": "HAM1",
"perf": 0.0156,
"cumul": 1.1165 
},
{
 "date":   9861,
"manager": "HAM1",
"perf": 0.0176,
"cumul": 1.1362 
},
{
 "date":   9892,
"manager": "HAM1",
"perf": 0.0212,
"cumul": 1.1603 
},
{
 "date":   9920,
"manager": "HAM1",
"perf": 0.0022,
"cumul": 1.1628 
},
{
 "date":   9951,
"manager": "HAM1",
"perf": 0.0094,
"cumul": 1.1738 
},
{
 "date":   9981,
"manager": "HAM1",
"perf": 0.0126,
"cumul": 1.1885 
},
{
 "date":  10012,
"manager": "HAM1",
"perf": 0.0438,
"cumul": 1.2406 
},
{
 "date":  10042,
"manager": "HAM1",
"perf": 0.0231,
"cumul": 1.2693 
},
{
 "date":  10073,
"manager": "HAM1",
"perf": 0.0154,
"cumul": 1.2888 
},
{
 "date":  10104,
"manager": "HAM1",
"perf": 0.0237,
"cumul": 1.3193 
},
{
 "date":  10134,
"manager": "HAM1",
"perf": 0.0219,
"cumul": 1.3482 
},
{
 "date":  10165,
"manager": "HAM1",
"perf": -0.0207,
"cumul": 1.3203 
},
{
 "date":  10195,
"manager": "HAM1",
"perf":  0.025,
"cumul": 1.3533 
},
{
 "date":  10226,
"manager": "HAM1",
"perf":  0.011,
"cumul": 1.3682 
},
{
 "date":  10257,
"manager": "HAM1",
"perf": 0.0056,
"cumul": 1.3759 
},
{
 "date":  10285,
"manager": "HAM1",
"perf": 0.0429,
"cumul": 1.4349 
},
{
 "date":  10316,
"manager": "HAM1",
"perf": 0.0362,
"cumul": 1.4869 
},
{
 "date":  10346,
"manager": "HAM1",
"perf": 0.0078,
"cumul": 1.4985 
},
{
 "date":  10377,
"manager": "HAM1",
"perf": -0.0231,
"cumul": 1.4638 
},
{
 "date":  10407,
"manager": "HAM1",
"perf": 0.0121,
"cumul": 1.4816 
},
{
 "date":  10438,
"manager": "HAM1",
"perf": -0.0215,
"cumul": 1.4497 
},
{
 "date":  10469,
"manager": "HAM1",
"perf": -0.0944,
"cumul": 1.3129 
},
{
 "date":  10499,
"manager": "HAM1",
"perf": 0.0248,
"cumul": 1.3454 
},
{
 "date":  10530,
"manager": "HAM1",
"perf": 0.0558,
"cumul": 1.4205 
},
{
 "date":  10560,
"manager": "HAM1",
"perf": 0.0126,
"cumul": 1.4384 
},
{
 "date":  10591,
"manager": "HAM1",
"perf": 0.0097,
"cumul": 1.4523 
},
{
 "date":  10622,
"manager": "HAM1",
"perf": -0.0093,
"cumul": 1.4388 
},
{
 "date":  10650,
"manager": "HAM1",
"perf": 0.0094,
"cumul": 1.4524 
},
{
 "date":  10681,
"manager": "HAM1",
"perf": 0.0462,
"cumul": 1.5195 
},
{
 "date":  10711,
"manager": "HAM1",
"perf":  0.051,
"cumul": 1.5969 
},
{
 "date":  10742,
"manager": "HAM1",
"perf": 0.0162,
"cumul": 1.6228 
},
{
 "date":  10772,
"manager": "HAM1",
"perf": 0.0326,
"cumul": 1.6757 
},
{
 "date":  10803,
"manager": "HAM1",
"perf": 0.0098,
"cumul": 1.6921 
},
{
 "date":  10834,
"manager": "HAM1",
"perf": -0.0165,
"cumul": 1.6642 
},
{
 "date":  10864,
"manager": "HAM1",
"perf": -0.0045,
"cumul": 1.6567 
},
{
 "date":  10895,
"manager": "HAM1",
"perf": -0.0006,
"cumul": 1.6557 
},
{
 "date":  10925,
"manager": "HAM1",
"perf": 0.0035,
"cumul": 1.6615 
},
{
 "date":  10956,
"manager": "HAM1",
"perf": 0.0147,
"cumul":  1.686 
},
{
 "date":  10987,
"manager": "HAM1",
"perf": -0.0102,
"cumul": 1.6688 
},
{
 "date":  11016,
"manager": "HAM1",
"perf": 0.0123,
"cumul": 1.6893 
},
{
 "date":  11047,
"manager": "HAM1",
"perf": 0.0575,
"cumul": 1.7864 
},
{
 "date":  11077,
"manager": "HAM1",
"perf": 0.0202,
"cumul": 1.8225 
},
{
 "date":  11108,
"manager": "HAM1",
"perf": 0.0339,
"cumul": 1.8843 
},
{
 "date":  11138,
"manager": "HAM1",
"perf": 0.0123,
"cumul": 1.9075 
},
{
 "date":  11169,
"manager": "HAM1",
"perf": 0.0049,
"cumul": 1.9168 
},
{
 "date":  11200,
"manager": "HAM1",
"perf": 0.0387,
"cumul":  1.991 
},
{
 "date":  11230,
"manager": "HAM1",
"perf": 0.0013,
"cumul": 1.9936 
},
{
 "date":  11261,
"manager": "HAM1",
"perf": -0.0077,
"cumul": 1.9782 
},
{
 "date":  11291,
"manager": "HAM1",
"perf": 0.0104,
"cumul": 1.9988 
},
{
 "date":  11322,
"manager": "HAM1",
"perf": -0.0068,
"cumul": 1.9852 
},
{
 "date":  11353,
"manager": "HAM1",
"perf": 0.0079,
"cumul": 2.0009 
},
{
 "date":  11381,
"manager": "HAM1",
"perf": 0.0082,
"cumul": 2.0173 
},
{
 "date":  11412,
"manager": "HAM1",
"perf": -0.0105,
"cumul": 1.9961 
},
{
 "date":  11442,
"manager": "HAM1",
"perf": 0.0345,
"cumul":  2.065 
},
{
 "date":  11473,
"manager": "HAM1",
"perf": 0.0579,
"cumul": 2.1845 
},
{
 "date":  11503,
"manager": "HAM1",
"perf": 0.0021,
"cumul": 2.1891 
},
{
 "date":  11534,
"manager": "HAM1",
"perf": 0.0207,
"cumul": 2.2344 
},
{
 "date":  11565,
"manager": "HAM1",
"perf": 0.0161,
"cumul": 2.2704 
},
{
 "date":  11595,
"manager": "HAM1",
"perf": -0.0312,
"cumul": 2.1996 
},
{
 "date":  11626,
"manager": "HAM1",
"perf": 0.0011,
"cumul":  2.202 
},
{
 "date":  11656,
"manager": "HAM1",
"perf":  0.034,
"cumul": 2.2769 
},
{
 "date":  11687,
"manager": "HAM1",
"perf": 0.0676,
"cumul": 2.4308 
},
{
 "date":  11718,
"manager": "HAM1",
"perf": 0.0135,
"cumul": 2.4636 
},
{
 "date":  11746,
"manager": "HAM1",
"perf": -0.0124,
"cumul": 2.4331 
},
{
 "date":  11777,
"manager": "HAM1",
"perf": 0.0063,
"cumul": 2.4484 
},
{
 "date":  11807,
"manager": "HAM1",
"perf": 0.0046,
"cumul": 2.4596 
},
{
 "date":  11838,
"manager": "HAM1",
"perf": -0.0015,
"cumul":  2.456 
},
{
 "date":  11868,
"manager": "HAM1",
"perf": -0.0241,
"cumul": 2.3968 
},
{
 "date":  11899,
"manager": "HAM1",
"perf": -0.0755,
"cumul": 2.2158 
},
{
 "date":  11930,
"manager": "HAM1",
"perf": 0.0077,
"cumul": 2.2329 
},
{
 "date":  11960,
"manager": "HAM1",
"perf": -0.0575,
"cumul": 2.1045 
},
{
 "date":  11991,
"manager": "HAM1",
"perf": 0.0297,
"cumul":  2.167 
},
{
 "date":  12021,
"manager": "HAM1",
"perf": 0.0661,
"cumul": 2.3102 
},
{
 "date":  12052,
"manager": "HAM1",
"perf": -0.0323,
"cumul": 2.2356 
},
{
 "date":  12083,
"manager": "HAM1",
"perf": -0.0412,
"cumul": 2.1435 
},
{
 "date":  12111,
"manager": "HAM1",
"perf": -0.0251,
"cumul": 2.0897 
},
{
 "date":  12142,
"manager": "HAM1",
"perf": 0.0364,
"cumul": 2.1658 
},
{
 "date":  12172,
"manager": "HAM1",
"perf": 0.0651,
"cumul": 2.3068 
},
{
 "date":  12203,
"manager": "HAM1",
"perf": 0.0337,
"cumul": 2.3845 
},
{
 "date":  12233,
"manager": "HAM1",
"perf": 0.0308,
"cumul": 2.4579 
},
{
 "date":  12264,
"manager": "HAM1",
"perf": 0.0176,
"cumul": 2.5012 
},
{
 "date":  12295,
"manager": "HAM1",
"perf": 0.0003,
"cumul": 2.5019 
},
{
 "date":  12325,
"manager": "HAM1",
"perf":  0.009,
"cumul": 2.5245 
},
{
 "date":  12356,
"manager": "HAM1",
"perf": 0.0481,
"cumul": 2.6459 
},
{
 "date":  12386,
"manager": "HAM1",
"perf": 0.0169,
"cumul": 2.6906 
},
{
 "date":  12417,
"manager": "HAM1",
"perf": 0.0275,
"cumul": 2.7646 
},
{
 "date":  12448,
"manager": "HAM1",
"perf": 0.0053,
"cumul": 2.7792 
},
{
 "date":  12477,
"manager": "HAM1",
"perf": -0.0001,
"cumul":  2.779 
},
{
 "date":  12508,
"manager": "HAM1",
"perf": 0.0087,
"cumul": 2.8031 
},
{
 "date":  12538,
"manager": "HAM1",
"perf": -0.0043,
"cumul": 2.7911 
},
{
 "date":  12569,
"manager": "HAM1",
"perf": 0.0082,
"cumul":  2.814 
},
{
 "date":  12599,
"manager": "HAM1",
"perf": 0.0259,
"cumul": 2.8869 
},
{
 "date":  12630,
"manager": "HAM1",
"perf":      0,
"cumul": 2.8869 
},
{
 "date":  12661,
"manager": "HAM1",
"perf": 0.0055,
"cumul": 2.9027 
},
{
 "date":  12691,
"manager": "HAM1",
"perf": 0.0088,
"cumul": 2.9283 
},
{
 "date":  12722,
"manager": "HAM1",
"perf": -0.0006,
"cumul": 2.9265 
},
{
 "date":  12752,
"manager": "HAM1",
"perf": 0.0394,
"cumul": 3.0418 
},
{
 "date":  12783,
"manager": "HAM1",
"perf":  0.044,
"cumul": 3.1757 
},
{
 "date":  12814,
"manager": "HAM1",
"perf": 0.0001,
"cumul":  3.176 
},
{
 "date":  12842,
"manager": "HAM1",
"perf": 0.0215,
"cumul": 3.2443 
},
{
 "date":  12873,
"manager": "HAM1",
"perf": -0.0207,
"cumul": 3.1771 
},
{
 "date":  12903,
"manager": "HAM1",
"perf": -0.0209,
"cumul": 3.1107 
},
{
 "date":  12934,
"manager": "HAM1",
"perf": 0.0043,
"cumul": 3.1241 
},
{
 "date":  12964,
"manager": "HAM1",
"perf": 0.0161,
"cumul": 3.1744 
},
{
 "date":  12995,
"manager": "HAM1",
"perf": 0.0091,
"cumul": 3.2033 
},
{
 "date":  13026,
"manager": "HAM1",
"perf": 0.0113,
"cumul": 3.2395 
},
{
 "date":  13056,
"manager": "HAM1",
"perf": 0.0261,
"cumul":  3.324 
},
{
 "date":  13087,
"manager": "HAM1",
"perf": -0.0187,
"cumul": 3.2619 
},
{
 "date":  13117,
"manager": "HAM1",
"perf": 0.0231,
"cumul": 3.3372 
},
{
 "date":  13148,
"manager": "HAM1",
"perf": 0.0261,
"cumul": 3.4243 
},
{
 "date":  13179,
"manager": "HAM1",
"perf": 0.0692,
"cumul": 3.6613 
},
{
 "date":  13207,
"manager": "HAM1",
"perf": 0.0145,
"cumul": 3.7144 
},
{
 "date":  13238,
"manager": "HAM1",
"perf": 0.0397,
"cumul": 3.8618 
},
{
 "date":  13268,
"manager": "HAM1",
"perf": -0.0011,
"cumul": 3.8576 
},
{
 "date":  13299,
"manager": "HAM1",
"perf": -0.0267,
"cumul": 3.7546 
},
{
 "date":  13329,
"manager": "HAM1",
"perf": 0.0216,
"cumul": 3.8357 
},
{
 "date":  13360,
"manager": "HAM1",
"perf": -0.0144,
"cumul": 3.7804 
},
{
 "date":  13391,
"manager": "HAM1",
"perf": 0.0161,
"cumul": 3.8413 
},
{
 "date":  13421,
"manager": "HAM1",
"perf": 0.0068,
"cumul": 3.8674 
},
{
 "date":  13452,
"manager": "HAM1",
"perf": 0.0427,
"cumul": 4.0326 
},
{
 "date":  13482,
"manager": "HAM1",
"perf": 0.0117,
"cumul": 4.0798 
},
{
 "date":  13513,
"manager": "HAM1",
"perf": 0.0115,
"cumul": 4.1267 
},
{
 "date":   9526,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9555,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9586,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9616,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9647,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9677,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9708,
"manager": "HAM2",
"perf": null,
"cumul":      1 
},
{
 "date":   9739,
"manager": "HAM2",
"perf": -0.0001,
"cumul": 0.9999 
},
{
 "date":   9769,
"manager": "HAM2",
"perf": 0.1002,
"cumul": 1.1001 
},
{
 "date":   9800,
"manager": "HAM2",
"perf": 0.0338,
"cumul": 1.1373 
},
{
 "date":   9830,
"manager": "HAM2",
"perf": 0.0737,
"cumul": 1.2211 
},
{
 "date":   9861,
"manager": "HAM2",
"perf": 0.0298,
"cumul": 1.2575 
},
{
 "date":   9892,
"manager": "HAM2",
"perf": 0.0794,
"cumul": 1.3573 
},
{
 "date":   9920,
"manager": "HAM2",
"perf": -0.0082,
"cumul": 1.3462 
},
{
 "date":   9951,
"manager": "HAM2",
"perf": -0.0269,
"cumul":   1.31 
},
{
 "date":   9981,
"manager": "HAM2",
"perf": -0.0061,
"cumul":  1.302 
},
{
 "date":  10012,
"manager": "HAM2",
"perf": 0.0539,
"cumul": 1.3722 
},
{
 "date":  10042,
"manager": "HAM2",
"perf": 0.0552,
"cumul": 1.4479 
},
{
 "date":  10073,
"manager": "HAM2",
"perf":  0.115,
"cumul": 1.6144 
},
{
 "date":  10104,
"manager": "HAM2",
"perf": -0.0197,
"cumul": 1.5826 
},
{
 "date":  10134,
"manager": "HAM2",
"perf": 0.0576,
"cumul": 1.6738 
},
{
 "date":  10165,
"manager": "HAM2",
"perf": -0.0222,
"cumul": 1.6366 
},
{
 "date":  10195,
"manager": "HAM2",
"perf": -0.0051,
"cumul": 1.6283 
},
{
 "date":  10226,
"manager": "HAM2",
"perf": 0.0192,
"cumul": 1.6595 
},
{
 "date":  10257,
"manager": "HAM2",
"perf": -0.0112,
"cumul": 1.6409 
},
{
 "date":  10285,
"manager": "HAM2",
"perf": 0.1007,
"cumul": 1.8062 
},
{
 "date":  10316,
"manager": "HAM2",
"perf": 0.0625,
"cumul": 1.9191 
},
{
 "date":  10346,
"manager": "HAM2",
"perf": -0.001,
"cumul": 1.9172 
},
{
 "date":  10377,
"manager": "HAM2",
"perf": -0.0107,
"cumul": 1.8966 
},
{
 "date":  10407,
"manager": "HAM2",
"perf": 0.0392,
"cumul":  1.971 
},
{
 "date":  10438,
"manager": "HAM2",
"perf": -0.0272,
"cumul": 1.9174 
},
{
 "date":  10469,
"manager": "HAM2",
"perf":      0,
"cumul": 1.9174 
},
{
 "date":  10499,
"manager": "HAM2",
"perf": -0.0046,
"cumul": 1.9086 
},
{
 "date":  10530,
"manager": "HAM2",
"perf": 0.0349,
"cumul": 1.9752 
},
{
 "date":  10560,
"manager": "HAM2",
"perf": 0.0699,
"cumul": 2.1132 
},
{
 "date":  10591,
"manager": "HAM2",
"perf": 0.0913,
"cumul": 2.3062 
},
{
 "date":  10622,
"manager": "HAM2",
"perf": 0.0787,
"cumul": 2.4877 
},
{
 "date":  10650,
"manager": "HAM2",
"perf": -0.023,
"cumul": 2.4305 
},
{
 "date":  10681,
"manager": "HAM2",
"perf": 0.1082,
"cumul": 2.6934 
},
{
 "date":  10711,
"manager": "HAM2",
"perf": 0.0166,
"cumul": 2.7381 
},
{
 "date":  10742,
"manager": "HAM2",
"perf": -0.0002,
"cumul": 2.7376 
},
{
 "date":  10772,
"manager": "HAM2",
"perf":  0.065,
"cumul": 2.9155 
},
{
 "date":  10803,
"manager": "HAM2",
"perf": 0.0279,
"cumul": 2.9969 
},
{
 "date":  10834,
"manager": "HAM2",
"perf": 0.0285,
"cumul": 3.0823 
},
{
 "date":  10864,
"manager": "HAM2",
"perf": 0.0332,
"cumul": 3.1846 
},
{
 "date":  10895,
"manager": "HAM2",
"perf": 0.0422,
"cumul":  3.319 
},
{
 "date":  10925,
"manager": "HAM2",
"perf": 0.0697,
"cumul": 3.5503 
},
{
 "date":  10956,
"manager": "HAM2",
"perf": 0.1449,
"cumul": 4.0648 
},
{
 "date":  10987,
"manager": "HAM2",
"perf": 0.0378,
"cumul": 4.2184 
},
{
 "date":  11016,
"manager": "HAM2",
"perf": 0.1556,
"cumul": 4.8748 
},
{
 "date":  11047,
"manager": "HAM2",
"perf": -0.0363,
"cumul": 4.6979 
},
{
 "date":  11077,
"manager": "HAM2",
"perf": -0.0098,
"cumul": 4.6518 
},
{
 "date":  11108,
"manager": "HAM2",
"perf": -0.0117,
"cumul": 4.5974 
},
{
 "date":  11138,
"manager": "HAM2",
"perf": 0.0105,
"cumul": 4.6457 
},
{
 "date":  11169,
"manager": "HAM2",
"perf": 0.0188,
"cumul":  4.733 
},
{
 "date":  11200,
"manager": "HAM2",
"perf": 0.0347,
"cumul": 4.8973 
},
{
 "date":  11230,
"manager": "HAM2",
"perf": -0.0297,
"cumul": 4.7518 
},
{
 "date":  11261,
"manager": "HAM2",
"perf": -0.0288,
"cumul":  4.615 
},
{
 "date":  11291,
"manager": "HAM2",
"perf": -0.022,
"cumul": 4.5134 
},
{
 "date":  11322,
"manager": "HAM2",
"perf":  0.019,
"cumul": 4.5992 
},
{
 "date":  11353,
"manager": "HAM2",
"perf": -0.0325,
"cumul": 4.4497 
},
{
 "date":  11381,
"manager": "HAM2",
"perf": -0.0193,
"cumul": 4.3638 
},
{
 "date":  11412,
"manager": "HAM2",
"perf": -0.0032,
"cumul": 4.3499 
},
{
 "date":  11442,
"manager": "HAM2",
"perf": -0.0019,
"cumul": 4.3416 
},
{
 "date":  11473,
"manager": "HAM2",
"perf": 0.0075,
"cumul": 4.3742 
},
{
 "date":  11503,
"manager": "HAM2",
"perf": -0.0207,
"cumul": 4.2836 
},
{
 "date":  11534,
"manager": "HAM2",
"perf": -0.0024,
"cumul": 4.2733 
},
{
 "date":  11565,
"manager": "HAM2",
"perf": 0.0083,
"cumul": 4.3088 
},
{
 "date":  11595,
"manager": "HAM2",
"perf": 0.0333,
"cumul": 4.4523 
},
{
 "date":  11626,
"manager": "HAM2",
"perf": -0.022,
"cumul": 4.3543 
},
{
 "date":  11656,
"manager": "HAM2",
"perf": 0.0082,
"cumul":   4.39 
},
{
 "date":  11687,
"manager": "HAM2",
"perf": -0.0003,
"cumul": 4.3887 
},
{
 "date":  11718,
"manager": "HAM2",
"perf": -0.0188,
"cumul": 4.3062 
},
{
 "date":  11746,
"manager": "HAM2",
"perf": -0.0371,
"cumul": 4.1465 
},
{
 "date":  11777,
"manager": "HAM2",
"perf": 0.0221,
"cumul": 4.2381 
},
{
 "date":  11807,
"manager": "HAM2",
"perf": -0.0116,
"cumul": 4.1889 
},
{
 "date":  11838,
"manager": "HAM2",
"perf": -0.0295,
"cumul": 4.0654 
},
{
 "date":  11868,
"manager": "HAM2",
"perf": -0.0338,
"cumul": 3.9279 
},
{
 "date":  11899,
"manager": "HAM2",
"perf": -0.0124,
"cumul": 3.8792 
},
{
 "date":  11930,
"manager": "HAM2",
"perf": -0.0004,
"cumul": 3.8777 
},
{
 "date":  11960,
"manager": "HAM2",
"perf": -0.0017,
"cumul": 3.8711 
},
{
 "date":  11991,
"manager": "HAM2",
"perf": 0.0043,
"cumul": 3.8877 
},
{
 "date":  12021,
"manager": "HAM2",
"perf": -0.0083,
"cumul": 3.8555 
},
{
 "date":  12052,
"manager": "HAM2",
"perf": -0.0022,
"cumul":  3.847 
},
{
 "date":  12083,
"manager": "HAM2",
"perf": -0.0003,
"cumul": 3.8458 
},
{
 "date":  12111,
"manager": "HAM2",
"perf": -0.0149,
"cumul": 3.7885 
},
{
 "date":  12142,
"manager": "HAM2",
"perf": -0.0056,
"cumul": 3.7673 
},
{
 "date":  12172,
"manager": "HAM2",
"perf": -0.0119,
"cumul": 3.7225 
},
{
 "date":  12203,
"manager": "HAM2",
"perf": 0.0515,
"cumul": 3.9142 
},
{
 "date":  12233,
"manager": "HAM2",
"perf": 0.0235,
"cumul": 4.0062 
},
{
 "date":  12264,
"manager": "HAM2",
"perf": 0.0234,
"cumul": 4.0999 
},
{
 "date":  12295,
"manager": "HAM2",
"perf": -0.0084,
"cumul": 4.0655 
},
{
 "date":  12325,
"manager": "HAM2",
"perf": -0.0053,
"cumul": 4.0439 
},
{
 "date":  12356,
"manager": "HAM2",
"perf": 0.0134,
"cumul": 4.0981 
},
{
 "date":  12386,
"manager": "HAM2",
"perf": 0.0114,
"cumul": 4.1448 
},
{
 "date":  12417,
"manager": "HAM2",
"perf": 0.0289,
"cumul": 4.2646 
},
{
 "date":  12448,
"manager": "HAM2",
"perf": 0.0191,
"cumul": 4.3461 
},
{
 "date":  12477,
"manager": "HAM2",
"perf": 0.0087,
"cumul": 4.3839 
},
{
 "date":  12508,
"manager": "HAM2",
"perf": 0.0128,
"cumul":   4.44 
},
{
 "date":  12538,
"manager": "HAM2",
"perf": 0.0082,
"cumul": 4.4764 
},
{
 "date":  12569,
"manager": "HAM2",
"perf": 0.0075,
"cumul":   4.51 
},
{
 "date":  12599,
"manager": "HAM2",
"perf": 0.0138,
"cumul": 4.5722 
},
{
 "date":  12630,
"manager": "HAM2",
"perf": 0.0042,
"cumul": 4.5914 
},
{
 "date":  12661,
"manager": "HAM2",
"perf": -0.0065,
"cumul": 4.5616 
},
{
 "date":  12691,
"manager": "HAM2",
"perf":   0.01,
"cumul": 4.6072 
},
{
 "date":  12722,
"manager": "HAM2",
"perf": 0.0147,
"cumul": 4.6749 
},
{
 "date":  12752,
"manager": "HAM2",
"perf": 0.0252,
"cumul": 4.7927 
},
{
 "date":  12783,
"manager": "HAM2",
"perf": 0.0083,
"cumul": 4.8325 
},
{
 "date":  12814,
"manager": "HAM2",
"perf": -0.0054,
"cumul": 4.8064 
},
{
 "date":  12842,
"manager": "HAM2",
"perf":  0.021,
"cumul": 4.9074 
},
{
 "date":  12873,
"manager": "HAM2",
"perf": -0.0069,
"cumul": 4.8735 
},
{
 "date":  12903,
"manager": "HAM2",
"perf": -0.0039,
"cumul": 4.8545 
},
{
 "date":  12934,
"manager": "HAM2",
"perf": -0.0139,
"cumul":  4.787 
},
{
 "date":  12964,
"manager": "HAM2",
"perf": 0.0194,
"cumul": 4.8799 
},
{
 "date":  12995,
"manager": "HAM2",
"perf": 0.0199,
"cumul":  4.977 
},
{
 "date":  13026,
"manager": "HAM2",
"perf": 0.0123,
"cumul": 5.0382 
},
{
 "date":  13056,
"manager": "HAM2",
"perf":  0.018,
"cumul": 5.1289 
},
{
 "date":  13087,
"manager": "HAM2",
"perf": -0.0186,
"cumul": 5.0335 
},
{
 "date":  13117,
"manager": "HAM2",
"perf": 0.0094,
"cumul": 5.0808 
},
{
 "date":  13148,
"manager": "HAM2",
"perf": 0.0085,
"cumul":  5.124 
},
{
 "date":  13179,
"manager": "HAM2",
"perf": 0.0812,
"cumul": 5.5401 
},
{
 "date":  13207,
"manager": "HAM2",
"perf": -0.0326,
"cumul": 5.3595 
},
{
 "date":  13238,
"manager": "HAM2",
"perf": 0.0151,
"cumul": 5.4404 
},
{
 "date":  13268,
"manager": "HAM2",
"perf": 0.0172,
"cumul":  5.534 
},
{
 "date":  13299,
"manager": "HAM2",
"perf": -0.0052,
"cumul": 5.5052 
},
{
 "date":  13329,
"manager": "HAM2",
"perf": -0.0116,
"cumul": 5.4413 
},
{
 "date":  13360,
"manager": "HAM2",
"perf": -0.0131,
"cumul":   5.37 
},
{
 "date":  13391,
"manager": "HAM2",
"perf": -0.0113,
"cumul": 5.3094 
},
{
 "date":  13421,
"manager": "HAM2",
"perf": -0.0231,
"cumul": 5.1867 
},
{
 "date":  13452,
"manager": "HAM2",
"perf": 0.0167,
"cumul": 5.2733 
},
{
 "date":  13482,
"manager": "HAM2",
"perf": 0.0206,
"cumul":  5.382 
},
{
 "date":  13513,
"manager": "HAM2",
"perf": -0.0062,
"cumul": 5.3486 
},
{
 "date":   9526,
"manager": "HAM3",
"perf": 0.0349,
"cumul": 1.0349 
},
{
 "date":   9555,
"manager": "HAM3",
"perf": 0.0351,
"cumul": 1.0712 
},
{
 "date":   9586,
"manager": "HAM3",
"perf": 0.0258,
"cumul": 1.0989 
},
{
 "date":   9616,
"manager": "HAM3",
"perf": 0.0449,
"cumul": 1.1482 
},
{
 "date":   9647,
"manager": "HAM3",
"perf": 0.0353,
"cumul": 1.1887 
},
{
 "date":   9677,
"manager": "HAM3",
"perf": -0.0303,
"cumul": 1.1527 
},
{
 "date":   9708,
"manager": "HAM3",
"perf": -0.0337,
"cumul": 1.1139 
},
{
 "date":   9739,
"manager": "HAM3",
"perf": 0.0461,
"cumul": 1.1652 
},
{
 "date":   9769,
"manager": "HAM3",
"perf": 0.0653,
"cumul": 1.2413 
},
{
 "date":   9800,
"manager": "HAM3",
"perf": 0.0395,
"cumul": 1.2903 
},
{
 "date":   9830,
"manager": "HAM3",
"perf": 0.0666,
"cumul": 1.3763 
},
{
 "date":   9861,
"manager": "HAM3",
"perf": 0.0214,
"cumul": 1.4057 
},
{
 "date":   9892,
"manager": "HAM3",
"perf": 0.0771,
"cumul": 1.5141 
},
{
 "date":   9920,
"manager": "HAM3",
"perf": -0.0374,
"cumul": 1.4575 
},
{
 "date":   9951,
"manager": "HAM3",
"perf": -0.0336,
"cumul": 1.4085 
},
{
 "date":   9981,
"manager": "HAM3",
"perf": 0.0286,
"cumul": 1.4488 
},
{
 "date":  10012,
"manager": "HAM3",
"perf": 0.0759,
"cumul": 1.5588 
},
{
 "date":  10042,
"manager": "HAM3",
"perf": 0.0054,
"cumul": 1.5672 
},
{
 "date":  10073,
"manager": "HAM3",
"perf": 0.1081,
"cumul": 1.7366 
},
{
 "date":  10104,
"manager": "HAM3",
"perf": -0.0028,
"cumul": 1.7317 
},
{
 "date":  10134,
"manager": "HAM3",
"perf": 0.0549,
"cumul": 1.8268 
},
{
 "date":  10165,
"manager": "HAM3",
"perf": -0.0354,
"cumul": 1.7621 
},
{
 "date":  10195,
"manager": "HAM3",
"perf": 0.0176,
"cumul": 1.7931 
},
{
 "date":  10226,
"manager": "HAM3",
"perf": -0.0003,
"cumul": 1.7926 
},
{
 "date":  10257,
"manager": "HAM3",
"perf": 0.0491,
"cumul": 1.8806 
},
{
 "date":  10285,
"manager": "HAM3",
"perf": 0.0466,
"cumul": 1.9683 
},
{
 "date":  10316,
"manager": "HAM3",
"perf": 0.0208,
"cumul": 2.0092 
},
{
 "date":  10346,
"manager": "HAM3",
"perf": 0.0234,
"cumul": 2.0562 
},
{
 "date":  10377,
"manager": "HAM3",
"perf": -0.0136,
"cumul": 2.0282 
},
{
 "date":  10407,
"manager": "HAM3",
"perf": 0.0395,
"cumul": 2.1084 
},
{
 "date":  10438,
"manager": "HAM3",
"perf": 0.0005,
"cumul": 2.1094 
},
{
 "date":  10469,
"manager": "HAM3",
"perf": -0.0718,
"cumul":  1.958 
},
{
 "date":  10499,
"manager": "HAM3",
"perf": 0.0665,
"cumul": 2.0882 
},
{
 "date":  10530,
"manager": "HAM3",
"perf": -0.0051,
"cumul": 2.0775 
},
{
 "date":  10560,
"manager": "HAM3",
"perf": 0.0555,
"cumul": 2.1928 
},
{
 "date":  10591,
"manager": "HAM3",
"perf": 0.0464,
"cumul": 2.2946 
},
{
 "date":  10622,
"manager": "HAM3",
"perf": 0.0269,
"cumul": 2.3563 
},
{
 "date":  10650,
"manager": "HAM3",
"perf": -0.053,
"cumul": 2.2314 
},
{
 "date":  10681,
"manager": "HAM3",
"perf": 0.0187,
"cumul": 2.2731 
},
{
 "date":  10711,
"manager": "HAM3",
"perf": 0.0417,
"cumul": 2.3679 
},
{
 "date":  10742,
"manager": "HAM3",
"perf": 0.0079,
"cumul": 2.3866 
},
{
 "date":  10772,
"manager": "HAM3",
"perf": 0.0547,
"cumul": 2.5172 
},
{
 "date":  10803,
"manager": "HAM3",
"perf": 0.0042,
"cumul": 2.5277 
},
{
 "date":  10834,
"manager": "HAM3",
"perf": 0.0122,
"cumul": 2.5586 
},
{
 "date":  10864,
"manager": "HAM3",
"perf": 0.0068,
"cumul":  2.576 
},
{
 "date":  10895,
"manager": "HAM3",
"perf": 0.0747,
"cumul": 2.7684 
},
{
 "date":  10925,
"manager": "HAM3",
"perf": 0.1074,
"cumul": 3.0657 
},
{
 "date":  10956,
"manager": "HAM3",
"perf":  0.058,
"cumul": 3.2435 
},
{
 "date":  10987,
"manager": "HAM3",
"perf": -0.005,
"cumul": 3.2273 
},
{
 "date":  11016,
"manager": "HAM3",
"perf": 0.1796,
"cumul":  3.807 
},
{
 "date":  11047,
"manager": "HAM3",
"perf": 0.0028,
"cumul": 3.8176 
},
{
 "date":  11077,
"manager": "HAM3",
"perf": -0.0127,
"cumul": 3.7691 
},
{
 "date":  11108,
"manager": "HAM3",
"perf": -0.0228,
"cumul": 3.6832 
},
{
 "date":  11138,
"manager": "HAM3",
"perf": 0.0407,
"cumul": 3.8331 
},
{
 "date":  11169,
"manager": "HAM3",
"perf": -0.0525,
"cumul": 3.6319 
},
{
 "date":  11200,
"manager": "HAM3",
"perf": 0.0795,
"cumul": 3.9206 
},
{
 "date":  11230,
"manager": "HAM3",
"perf": -0.0573,
"cumul": 3.6959 
},
{
 "date":  11261,
"manager": "HAM3",
"perf": 0.0162,
"cumul": 3.7558 
},
{
 "date":  11291,
"manager": "HAM3",
"perf": -0.0368,
"cumul": 3.6176 
},
{
 "date":  11322,
"manager": "HAM3",
"perf": 0.0169,
"cumul": 3.6787 
},
{
 "date":  11353,
"manager": "HAM3",
"perf": 0.0262,
"cumul": 3.7751 
},
{
 "date":  11381,
"manager": "HAM3",
"perf": -0.0355,
"cumul": 3.6411 
},
{
 "date":  11412,
"manager": "HAM3",
"perf": -0.011,
"cumul": 3.6011 
},
{
 "date":  11442,
"manager": "HAM3",
"perf": 0.0132,
"cumul": 3.6486 
},
{
 "date":  11473,
"manager": "HAM3",
"perf": -0.0053,
"cumul": 3.6293 
},
{
 "date":  11503,
"manager": "HAM3",
"perf": -0.0237,
"cumul": 3.5432 
},
{
 "date":  11534,
"manager": "HAM3",
"perf": -0.0022,
"cumul": 3.5354 
},
{
 "date":  11565,
"manager": "HAM3",
"perf": -0.0246,
"cumul": 3.4485 
},
{
 "date":  11595,
"manager": "HAM3",
"perf": -0.0068,
"cumul":  3.425 
},
{
 "date":  11626,
"manager": "HAM3",
"perf": -0.0205,
"cumul": 3.3548 
},
{
 "date":  11656,
"manager": "HAM3",
"perf": 0.0248,
"cumul":  3.438 
},
{
 "date":  11687,
"manager": "HAM3",
"perf": 0.0018,
"cumul": 3.4442 
},
{
 "date":  11718,
"manager": "HAM3",
"perf": -0.0145,
"cumul": 3.3943 
},
{
 "date":  11746,
"manager": "HAM3",
"perf": -0.0414,
"cumul": 3.2537 
},
{
 "date":  11777,
"manager": "HAM3",
"perf": 0.0207,
"cumul": 3.3211 
},
{
 "date":  11807,
"manager": "HAM3",
"perf": -0.0253,
"cumul": 3.2371 
},
{
 "date":  11838,
"manager": "HAM3",
"perf": -0.0024,
"cumul": 3.2293 
},
{
 "date":  11868,
"manager": "HAM3",
"perf": -0.0451,
"cumul": 3.0837 
},
{
 "date":  11899,
"manager": "HAM3",
"perf": -0.034,
"cumul": 2.9788 
},
{
 "date":  11930,
"manager": "HAM3",
"perf": 0.0024,
"cumul":  2.986 
},
{
 "date":  11960,
"manager": "HAM3",
"perf": -0.0439,
"cumul": 2.8549 
},
{
 "date":  11991,
"manager": "HAM3",
"perf": 0.0102,
"cumul":  2.884 
},
{
 "date":  12021,
"manager": "HAM3",
"perf":  0.035,
"cumul": 2.9849 
},
{
 "date":  12052,
"manager": "HAM3",
"perf": -0.0652,
"cumul": 2.7903 
},
{
 "date":  12083,
"manager": "HAM3",
"perf": -0.0015,
"cumul": 2.7861 
},
{
 "date":  12111,
"manager": "HAM3",
"perf": 0.0021,
"cumul":  2.792 
},
{
 "date":  12142,
"manager": "HAM3",
"perf": 0.0111,
"cumul":  2.823 
},
{
 "date":  12172,
"manager": "HAM3",
"perf": 0.0525,
"cumul": 2.9712 
},
{
 "date":  12203,
"manager": "HAM3",
"perf": 0.0423,
"cumul": 3.0969 
},
{
 "date":  12233,
"manager": "HAM3",
"perf": 0.0109,
"cumul": 3.1306 
},
{
 "date":  12264,
"manager": "HAM3",
"perf": 0.0086,
"cumul": 3.1575 
},
{
 "date":  12295,
"manager": "HAM3",
"perf": 0.0302,
"cumul": 3.2529 
},
{
 "date":  12325,
"manager": "HAM3",
"perf": -0.0025,
"cumul": 3.2448 
},
{
 "date":  12356,
"manager": "HAM3",
"perf": 0.0605,
"cumul": 3.4411 
},
{
 "date":  12386,
"manager": "HAM3",
"perf": 0.0118,
"cumul": 3.4817 
},
{
 "date":  12417,
"manager": "HAM3",
"perf": 0.0095,
"cumul": 3.5148 
},
{
 "date":  12448,
"manager": "HAM3",
"perf": 0.0054,
"cumul": 3.5337 
},
{
 "date":  12477,
"manager": "HAM3",
"perf": 0.0143,
"cumul": 3.5843 
},
{
 "date":  12508,
"manager": "HAM3",
"perf": -0.0038,
"cumul": 3.5706 
},
{
 "date":  12538,
"manager": "HAM3",
"perf":  -0.02,
"cumul": 3.4992 
},
{
 "date":  12569,
"manager": "HAM3",
"perf": -0.0067,
"cumul": 3.4758 
},
{
 "date":  12599,
"manager": "HAM3",
"perf":  0.001,
"cumul": 3.4793 
},
{
 "date":  12630,
"manager": "HAM3",
"perf": -0.0347,
"cumul": 3.3585 
},
{
 "date":  12661,
"manager": "HAM3",
"perf": -0.0056,
"cumul": 3.3397 
},
{
 "date":  12691,
"manager": "HAM3",
"perf": -0.0032,
"cumul":  3.329 
},
{
 "date":  12722,
"manager": "HAM3",
"perf": -0.0011,
"cumul": 3.3254 
},
{
 "date":  12752,
"manager": "HAM3",
"perf": 0.0554,
"cumul": 3.5096 
},
{
 "date":  12783,
"manager": "HAM3",
"perf": 0.0181,
"cumul": 3.5731 
},
{
 "date":  12814,
"manager": "HAM3",
"perf": 0.0073,
"cumul": 3.5992 
},
{
 "date":  12842,
"manager": "HAM3",
"perf": 0.0417,
"cumul": 3.7493 
},
{
 "date":  12873,
"manager": "HAM3",
"perf": 0.0093,
"cumul": 3.7842 
},
{
 "date":  12903,
"manager": "HAM3",
"perf": -0.0019,
"cumul":  3.777 
},
{
 "date":  12934,
"manager": "HAM3",
"perf": 0.0233,
"cumul":  3.865 
},
{
 "date":  12964,
"manager": "HAM3",
"perf": 0.0035,
"cumul": 3.8785 
},
{
 "date":  12995,
"manager": "HAM3",
"perf": 0.0203,
"cumul": 3.9572 
},
{
 "date":  13026,
"manager": "HAM3",
"perf": -0.002,
"cumul": 3.9493 
},
{
 "date":  13056,
"manager": "HAM3",
"perf": 0.0197,
"cumul": 4.0271 
},
{
 "date":  13087,
"manager": "HAM3",
"perf": -0.0111,
"cumul": 3.9824 
},
{
 "date":  13117,
"manager": "HAM3",
"perf": 0.0162,
"cumul": 4.0469 
},
{
 "date":  13148,
"manager": "HAM3",
"perf": 0.0181,
"cumul": 4.1202 
},
{
 "date":  13179,
"manager": "HAM3",
"perf": 0.0351,
"cumul": 4.2648 
},
{
 "date":  13207,
"manager": "HAM3",
"perf": 0.0266,
"cumul": 4.3783 
},
{
 "date":  13238,
"manager": "HAM3",
"perf": 0.0119,
"cumul": 4.4304 
},
{
 "date":  13268,
"manager": "HAM3",
"perf": 0.0031,
"cumul": 4.4441 
},
{
 "date":  13299,
"manager": "HAM3",
"perf": -0.0212,
"cumul": 4.3499 
},
{
 "date":  13329,
"manager": "HAM3",
"perf": -0.0189,
"cumul": 4.2677 
},
{
 "date":  13360,
"manager": "HAM3",
"perf": 0.0102,
"cumul": 4.3112 
},
{
 "date":  13391,
"manager": "HAM3",
"perf": 0.0253,
"cumul": 4.4203 
},
{
 "date":  13421,
"manager": "HAM3",
"perf": 0.0072,
"cumul": 4.4521 
},
{
 "date":  13452,
"manager": "HAM3",
"perf": 0.0183,
"cumul": 4.5336 
},
{
 "date":  13482,
"manager": "HAM3",
"perf": 0.0269,
"cumul": 4.6555 
},
{
 "date":  13513,
"manager": "HAM3",
"perf":  0.011,
"cumul": 4.7067 
},
{
 "date":   9526,
"manager": "HAM4",
"perf": 0.0222,
"cumul": 1.0222 
},
{
 "date":   9555,
"manager": "HAM4",
"perf": 0.0195,
"cumul": 1.0421 
},
{
 "date":   9586,
"manager": "HAM4",
"perf": -0.0098,
"cumul": 1.0319 
},
{
 "date":   9616,
"manager": "HAM4",
"perf": 0.0236,
"cumul": 1.0563 
},
{
 "date":   9647,
"manager": "HAM4",
"perf": 0.0028,
"cumul": 1.0592 
},
{
 "date":   9677,
"manager": "HAM4",
"perf": -0.0019,
"cumul": 1.0572 
},
{
 "date":   9708,
"manager": "HAM4",
"perf": -0.0446,
"cumul": 1.0101 
},
{
 "date":   9739,
"manager": "HAM4",
"perf": 0.0351,
"cumul": 1.0455 
},
{
 "date":   9769,
"manager": "HAM4",
"perf": 0.0757,
"cumul": 1.1247 
},
{
 "date":   9800,
"manager": "HAM4",
"perf": -0.018,
"cumul": 1.1044 
},
{
 "date":   9830,
"manager": "HAM4",
"perf": 0.0458,
"cumul":  1.155 
},
{
 "date":   9861,
"manager": "HAM4",
"perf": 0.0439,
"cumul": 1.2057 
},
{
 "date":   9892,
"manager": "HAM4",
"perf": 0.0437,
"cumul": 1.2584 
},
{
 "date":   9920,
"manager": "HAM4",
"perf": 0.0312,
"cumul": 1.2977 
},
{
 "date":   9951,
"manager": "HAM4",
"perf": 0.0113,
"cumul": 1.3123 
},
{
 "date":   9981,
"manager": "HAM4",
"perf": 0.0354,
"cumul": 1.3588 
},
{
 "date":  10012,
"manager": "HAM4",
"perf": 0.0789,
"cumul":  1.466 
},
{
 "date":  10042,
"manager": "HAM4",
"perf": 0.0412,
"cumul": 1.5264 
},
{
 "date":  10073,
"manager": "HAM4",
"perf": 0.0794,
"cumul": 1.6476 
},
{
 "date":  10104,
"manager": "HAM4",
"perf": 0.0143,
"cumul": 1.6711 
},
{
 "date":  10134,
"manager": "HAM4",
"perf": 0.0217,
"cumul": 1.7074 
},
{
 "date":  10165,
"manager": "HAM4",
"perf": 0.0056,
"cumul":  1.717 
},
{
 "date":  10195,
"manager": "HAM4",
"perf": -0.0067,
"cumul": 1.7055 
},
{
 "date":  10226,
"manager": "HAM4",
"perf": 0.0116,
"cumul": 1.7252 
},
{
 "date":  10257,
"manager": "HAM4",
"perf": -0.0041,
"cumul": 1.7182 
},
{
 "date":  10285,
"manager": "HAM4",
"perf": 0.0324,
"cumul": 1.7738 
},
{
 "date":  10316,
"manager": "HAM4",
"perf": 0.0404,
"cumul": 1.8455 
},
{
 "date":  10346,
"manager": "HAM4",
"perf": 0.0242,
"cumul": 1.8902 
},
{
 "date":  10377,
"manager": "HAM4",
"perf": -0.0047,
"cumul": 1.8813 
},
{
 "date":  10407,
"manager": "HAM4",
"perf": -0.0133,
"cumul": 1.8563 
},
{
 "date":  10438,
"manager": "HAM4",
"perf": -0.0723,
"cumul": 1.7221 
},
{
 "date":  10469,
"manager": "HAM4",
"perf": -0.1759,
"cumul": 1.4191 
},
{
 "date":  10499,
"manager": "HAM4",
"perf": 0.0549,
"cumul": 1.4971 
},
{
 "date":  10530,
"manager": "HAM4",
"perf": -0.0503,
"cumul": 1.4218 
},
{
 "date":  10560,
"manager": "HAM4",
"perf": 0.0887,
"cumul": 1.5479 
},
{
 "date":  10591,
"manager": "HAM4",
"perf": -0.0108,
"cumul": 1.5311 
},
{
 "date":  10622,
"manager": "HAM4",
"perf":  0.041,
"cumul": 1.5939 
},
{
 "date":  10650,
"manager": "HAM4",
"perf": -0.0549,
"cumul": 1.5064 
},
{
 "date":  10681,
"manager": "HAM4",
"perf": -0.0615,
"cumul": 1.4138 
},
{
 "date":  10711,
"manager": "HAM4",
"perf": 0.0684,
"cumul": 1.5105 
},
{
 "date":  10742,
"manager": "HAM4",
"perf": 0.0635,
"cumul": 1.6064 
},
{
 "date":  10772,
"manager": "HAM4",
"perf": 0.0093,
"cumul": 1.6213 
},
{
 "date":  10803,
"manager": "HAM4",
"perf": 0.0249,
"cumul": 1.6617 
},
{
 "date":  10834,
"manager": "HAM4",
"perf": -0.0407,
"cumul": 1.5941 
},
{
 "date":  10864,
"manager": "HAM4",
"perf": -0.0231,
"cumul": 1.5572 
},
{
 "date":  10895,
"manager": "HAM4",
"perf": 0.0253,
"cumul": 1.5966 
},
{
 "date":  10925,
"manager": "HAM4",
"perf": -0.0275,
"cumul": 1.5527 
},
{
 "date":  10956,
"manager": "HAM4",
"perf":  0.009,
"cumul": 1.5667 
},
{
 "date":  10987,
"manager": "HAM4",
"perf": 0.0424,
"cumul": 1.6331 
},
{
 "date":  11016,
"manager": "HAM4",
"perf": 0.0469,
"cumul": 1.7097 
},
{
 "date":  11047,
"manager": "HAM4",
"perf": -0.0267,
"cumul": 1.6641 
},
{
 "date":  11077,
"manager": "HAM4",
"perf": -0.0561,
"cumul": 1.5707 
},
{
 "date":  11108,
"manager": "HAM4",
"perf": 0.0107,
"cumul": 1.5875 
},
{
 "date":  11138,
"manager": "HAM4",
"perf": 0.0666,
"cumul": 1.6933 
},
{
 "date":  11169,
"manager": "HAM4",
"perf": -0.0266,
"cumul": 1.6482 
},
{
 "date":  11200,
"manager": "HAM4",
"perf":  0.055,
"cumul": 1.7389 
},
{
 "date":  11230,
"manager": "HAM4",
"perf": 0.0556,
"cumul": 1.8356 
},
{
 "date":  11261,
"manager": "HAM4",
"perf": -0.0819,
"cumul": 1.6852 
},
{
 "date":  11291,
"manager": "HAM4",
"perf": -0.0736,
"cumul": 1.5612 
},
{
 "date":  11322,
"manager": "HAM4",
"perf": 0.0466,
"cumul": 1.6339 
},
{
 "date":  11353,
"manager": "HAM4",
"perf": 0.0864,
"cumul": 1.7751 
},
{
 "date":  11381,
"manager": "HAM4",
"perf": -0.053,
"cumul":  1.681 
},
{
 "date":  11412,
"manager": "HAM4",
"perf": -0.0155,
"cumul":  1.655 
},
{
 "date":  11442,
"manager": "HAM4",
"perf": 0.0277,
"cumul": 1.7008 
},
{
 "date":  11473,
"manager": "HAM4",
"perf": 0.1508,
"cumul": 1.9573 
},
{
 "date":  11503,
"manager": "HAM4",
"perf": -0.0782,
"cumul": 1.8042 
},
{
 "date":  11534,
"manager": "HAM4",
"perf": -0.0556,
"cumul": 1.7039 
},
{
 "date":  11565,
"manager": "HAM4",
"perf": -0.0828,
"cumul": 1.5628 
},
{
 "date":  11595,
"manager": "HAM4",
"perf": -0.1075,
"cumul": 1.3948 
},
{
 "date":  11626,
"manager": "HAM4",
"perf": 0.0467,
"cumul":   1.46 
},
{
 "date":  11656,
"manager": "HAM4",
"perf": 0.0733,
"cumul":  1.567 
},
{
 "date":  11687,
"manager": "HAM4",
"perf": 0.1139,
"cumul": 1.7455 
},
{
 "date":  11718,
"manager": "HAM4",
"perf": -0.0344,
"cumul": 1.6854 
},
{
 "date":  11746,
"manager": "HAM4",
"perf": -0.0253,
"cumul": 1.6428 
},
{
 "date":  11777,
"manager": "HAM4",
"perf": 0.1378,
"cumul": 1.8692 
},
{
 "date":  11807,
"manager": "HAM4",
"perf": 0.0608,
"cumul": 1.9828 
},
{
 "date":  11838,
"manager": "HAM4",
"perf": 0.0018,
"cumul": 1.9864 
},
{
 "date":  11868,
"manager": "HAM4",
"perf": -0.0473,
"cumul": 1.8924 
},
{
 "date":  11899,
"manager": "HAM4",
"perf": -0.1406,
"cumul": 1.6263 
},
{
 "date":  11930,
"manager": "HAM4",
"perf": -0.0192,
"cumul": 1.5951 
},
{
 "date":  11960,
"manager": "HAM4",
"perf": -0.111,
"cumul": 1.4181 
},
{
 "date":  11991,
"manager": "HAM4",
"perf": 0.0091,
"cumul":  1.431 
},
{
 "date":  12021,
"manager": "HAM4",
"perf":  0.081,
"cumul": 1.5469 
},
{
 "date":  12052,
"manager": "HAM4",
"perf": 0.0354,
"cumul": 1.6016 
},
{
 "date":  12083,
"manager": "HAM4",
"perf": -0.0342,
"cumul": 1.5469 
},
{
 "date":  12111,
"manager": "HAM4",
"perf": -0.0047,
"cumul": 1.5396 
},
{
 "date":  12142,
"manager": "HAM4",
"perf": 0.0252,
"cumul": 1.5784 
},
{
 "date":  12172,
"manager": "HAM4",
"perf": 0.1147,
"cumul": 1.7594 
},
{
 "date":  12203,
"manager": "HAM4",
"perf": 0.0894,
"cumul": 1.9167 
},
{
 "date":  12233,
"manager": "HAM4",
"perf":  0.048,
"cumul": 2.0087 
},
{
 "date":  12264,
"manager": "HAM4",
"perf": 0.0321,
"cumul": 2.0732 
},
{
 "date":  12295,
"manager": "HAM4",
"perf": -0.0083,
"cumul":  2.056 
},
{
 "date":  12325,
"manager": "HAM4",
"perf": 0.0092,
"cumul": 2.0749 
},
{
 "date":  12356,
"manager": "HAM4",
"perf": 0.0634,
"cumul": 2.2065 
},
{
 "date":  12386,
"manager": "HAM4",
"perf": 0.0861,
"cumul": 2.3964 
},
{
 "date":  12417,
"manager": "HAM4",
"perf": 0.0488,
"cumul": 2.5134 
},
{
 "date":  12448,
"manager": "HAM4",
"perf": 0.0132,
"cumul": 2.5466 
},
{
 "date":  12477,
"manager": "HAM4",
"perf": 0.0441,
"cumul": 2.6589 
},
{
 "date":  12508,
"manager": "HAM4",
"perf": 0.0206,
"cumul": 2.7136 
},
{
 "date":  12538,
"manager": "HAM4",
"perf": -0.0859,
"cumul": 2.4805 
},
{
 "date":  12569,
"manager": "HAM4",
"perf": -0.018,
"cumul": 2.4359 
},
{
 "date":  12599,
"manager": "HAM4",
"perf": 0.0046,
"cumul": 2.4471 
},
{
 "date":  12630,
"manager": "HAM4",
"perf": -0.0337,
"cumul": 2.3646 
},
{
 "date":  12661,
"manager": "HAM4",
"perf": 0.0304,
"cumul": 2.4365 
},
{
 "date":  12691,
"manager": "HAM4",
"perf": 0.0406,
"cumul": 2.5354 
},
{
 "date":  12722,
"manager": "HAM4",
"perf": -0.0069,
"cumul": 2.5179 
},
{
 "date":  12752,
"manager": "HAM4",
"perf": 0.0854,
"cumul":  2.733 
},
{
 "date":  12783,
"manager": "HAM4",
"perf": 0.0469,
"cumul": 2.8611 
},
{
 "date":  12814,
"manager": "HAM4",
"perf": 0.0042,
"cumul": 2.8732 
},
{
 "date":  12842,
"manager": "HAM4",
"perf": -0.0318,
"cumul": 2.7818 
},
{
 "date":  12873,
"manager": "HAM4",
"perf": -0.0218,
"cumul": 2.7212 
},
{
 "date":  12903,
"manager": "HAM4",
"perf": -0.0094,
"cumul": 2.6956 
},
{
 "date":  12934,
"manager": "HAM4",
"perf": 0.0125,
"cumul": 2.7293 
},
{
 "date":  12964,
"manager": "HAM4",
"perf":  0.072,
"cumul": 2.9258 
},
{
 "date":  12995,
"manager": "HAM4",
"perf": 0.0632,
"cumul": 3.1107 
},
{
 "date":  13026,
"manager": "HAM4",
"perf": -0.0262,
"cumul": 3.0292 
},
{
 "date":  13056,
"manager": "HAM4",
"perf": -0.0332,
"cumul": 2.9286 
},
{
 "date":  13087,
"manager": "HAM4",
"perf": -0.0293,
"cumul": 2.8428 
},
{
 "date":  13117,
"manager": "HAM4",
"perf": 0.0637,
"cumul": 3.0239 
},
{
 "date":  13148,
"manager": "HAM4",
"perf": 0.0352,
"cumul": 3.1303 
},
{
 "date":  13179,
"manager": "HAM4",
"perf": 0.0552,
"cumul": 3.3031 
},
{
 "date":  13207,
"manager": "HAM4",
"perf": -0.0539,
"cumul": 3.1251 
},
{
 "date":  13238,
"manager": "HAM4",
"perf": 0.0107,
"cumul": 3.1585 
},
{
 "date":  13268,
"manager": "HAM4",
"perf":  0.018,
"cumul": 3.2154 
},
{
 "date":  13299,
"manager": "HAM4",
"perf": -0.0184,
"cumul": 3.1562 
},
{
 "date":  13329,
"manager": "HAM4",
"perf": 0.0154,
"cumul": 3.2048 
},
{
 "date":  13360,
"manager": "HAM4",
"perf": -0.012,
"cumul": 3.1664 
},
{
 "date":  13391,
"manager": "HAM4",
"perf": -0.0183,
"cumul": 3.1084 
},
{
 "date":  13421,
"manager": "HAM4",
"perf": 0.0197,
"cumul": 3.1697 
},
{
 "date":  13452,
"manager": "HAM4",
"perf": 0.0518,
"cumul": 3.3338 
},
{
 "date":  13482,
"manager": "HAM4",
"perf": 0.0373,
"cumul": 3.4582 
},
{
 "date":  13513,
"manager": "HAM4",
"perf": 0.0206,
"cumul": 3.5294 
},
{
 "date":   9526,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9555,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9586,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9616,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9647,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9677,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9708,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9739,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9769,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9800,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9830,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9861,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9892,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9920,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9951,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":   9981,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10012,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10042,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10073,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10104,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10134,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10165,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10195,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10226,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10257,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10285,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10316,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10346,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10377,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10407,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10438,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10469,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10499,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10530,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10560,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10591,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10622,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10650,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10681,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10711,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10742,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10772,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10803,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10834,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10864,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10895,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10925,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10956,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  10987,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11016,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11047,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11077,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11108,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11138,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11169,
"manager": "HAM5",
"perf": null,
"cumul":      1 
},
{
 "date":  11200,
"manager": "HAM5",
"perf": 0.1747,
"cumul": 1.1747 
},
{
 "date":  11230,
"manager": "HAM5",
"perf": -0.0215,
"cumul": 1.1494 
},
{
 "date":  11261,
"manager": "HAM5",
"perf": -0.1062,
"cumul": 1.0274 
},
{
 "date":  11291,
"manager": "HAM5",
"perf": 0.0014,
"cumul": 1.0288 
},
{
 "date":  11322,
"manager": "HAM5",
"perf": 0.0807,
"cumul": 1.1118 
},
{
 "date":  11353,
"manager": "HAM5",
"perf": -0.0941,
"cumul": 1.0072 
},
{
 "date":  11381,
"manager": "HAM5",
"perf": 0.0105,
"cumul": 1.0178 
},
{
 "date":  11412,
"manager": "HAM5",
"perf": 0.0063,
"cumul": 1.0242 
},
{
 "date":  11442,
"manager": "HAM5",
"perf": 0.0139,
"cumul": 1.0384 
},
{
 "date":  11473,
"manager": "HAM5",
"perf": 0.0213,
"cumul": 1.0606 
},
{
 "date":  11503,
"manager": "HAM5",
"perf": -0.0225,
"cumul": 1.0367 
},
{
 "date":  11534,
"manager": "HAM5",
"perf": -0.0003,
"cumul": 1.0364 
},
{
 "date":  11565,
"manager": "HAM5",
"perf": -0.077,
"cumul": 0.95658 
},
{
 "date":  11595,
"manager": "HAM5",
"perf": -0.007,
"cumul": 0.94988 
},
{
 "date":  11626,
"manager": "HAM5",
"perf": -0.132,
"cumul": 0.8245 
},
{
 "date":  11656,
"manager": "HAM5",
"perf":  0.024,
"cumul": 0.84429 
},
{
 "date":  11687,
"manager": "HAM5",
"perf": 0.0484,
"cumul": 0.88515 
},
{
 "date":  11718,
"manager": "HAM5",
"perf": 0.0846,
"cumul": 0.96004 
},
{
 "date":  11746,
"manager": "HAM5",
"perf": -0.0086,
"cumul": 0.95178 
},
{
 "date":  11777,
"manager": "HAM5",
"perf": -0.0724,
"cumul": 0.88287 
},
{
 "date":  11807,
"manager": "HAM5",
"perf": 0.0459,
"cumul": 0.92339 
},
{
 "date":  11838,
"manager": "HAM5",
"perf": -0.0543,
"cumul": 0.87325 
},
{
 "date":  11868,
"manager": "HAM5",
"perf": -0.0471,
"cumul": 0.83212 
},
{
 "date":  11899,
"manager": "HAM5",
"perf": -0.069,
"cumul": 0.77471 
},
{
 "date":  11930,
"manager": "HAM5",
"perf": 0.0775,
"cumul": 0.83475 
},
{
 "date":  11960,
"manager": "HAM5",
"perf": -0.042,
"cumul": 0.79969 
},
{
 "date":  11991,
"manager": "HAM5",
"perf": -0.0307,
"cumul": 0.77514 
},
{
 "date":  12021,
"manager": "HAM5",
"perf": 0.0153,
"cumul":  0.787 
},
{
 "date":  12052,
"manager": "HAM5",
"perf":  0.003,
"cumul": 0.78936 
},
{
 "date":  12083,
"manager": "HAM5",
"perf": -0.0014,
"cumul": 0.78825 
},
{
 "date":  12111,
"manager": "HAM5",
"perf": -0.0067,
"cumul": 0.78297 
},
{
 "date":  12142,
"manager": "HAM5",
"perf": 0.0451,
"cumul": 0.81828 
},
{
 "date":  12172,
"manager": "HAM5",
"perf": 0.0135,
"cumul": 0.82933 
},
{
 "date":  12203,
"manager": "HAM5",
"perf": 0.0624,
"cumul": 0.88108 
},
{
 "date":  12233,
"manager": "HAM5",
"perf": 0.0572,
"cumul": 0.93148 
},
{
 "date":  12264,
"manager": "HAM5",
"perf": -0.0404,
"cumul": 0.89385 
},
{
 "date":  12295,
"manager": "HAM5",
"perf": -0.0114,
"cumul": 0.88366 
},
{
 "date":  12325,
"manager": "HAM5",
"perf": 0.0368,
"cumul": 0.91617 
},
{
 "date":  12356,
"manager": "HAM5",
"perf": 0.0587,
"cumul": 0.96995 
},
{
 "date":  12386,
"manager": "HAM5",
"perf": 0.0315,
"cumul": 1.0005 
},
{
 "date":  12417,
"manager": "HAM5",
"perf": -0.0416,
"cumul": 0.95889 
},
{
 "date":  12448,
"manager": "HAM5",
"perf": -0.0024,
"cumul": 0.95659 
},
{
 "date":  12477,
"manager": "HAM5",
"perf": 0.0294,
"cumul": 0.98471 
},
{
 "date":  12508,
"manager": "HAM5",
"perf": -0.0062,
"cumul": 0.9786 
},
{
 "date":  12538,
"manager": "HAM5",
"perf": -0.0386,
"cumul": 0.94083 
},
{
 "date":  12569,
"manager": "HAM5",
"perf": 0.0145,
"cumul": 0.95447 
},
{
 "date":  12599,
"manager": "HAM5",
"perf": 0.0067,
"cumul": 0.96087 
},
{
 "date":  12630,
"manager": "HAM5",
"perf": -0.0228,
"cumul": 0.93896 
},
{
 "date":  12661,
"manager": "HAM5",
"perf": -0.0267,
"cumul": 0.91389 
},
{
 "date":  12691,
"manager": "HAM5",
"perf": 0.0359,
"cumul": 0.9467 
},
{
 "date":  12722,
"manager": "HAM5",
"perf": -0.0113,
"cumul":  0.936 
},
{
 "date":  12752,
"manager": "HAM5",
"perf": 0.0393,
"cumul": 0.97278 
},
{
 "date":  12783,
"manager": "HAM5",
"perf": 0.0544,
"cumul": 1.0257 
},
{
 "date":  12814,
"manager": "HAM5",
"perf": -0.0004,
"cumul": 1.0253 
},
{
 "date":  12842,
"manager": "HAM5",
"perf": 0.0063,
"cumul": 1.0318 
},
{
 "date":  12873,
"manager": "HAM5",
"perf": -0.0099,
"cumul": 1.0215 
},
{
 "date":  12903,
"manager": "HAM5",
"perf": -0.0294,
"cumul": 0.99151 
},
{
 "date":  12934,
"manager": "HAM5",
"perf": 0.0309,
"cumul": 1.0221 
},
{
 "date":  12964,
"manager": "HAM5",
"perf": 0.0033,
"cumul": 1.0255 
},
{
 "date":  12995,
"manager": "HAM5",
"perf": 0.0357,
"cumul": 1.0621 
},
{
 "date":  13026,
"manager": "HAM5",
"perf": 0.0265,
"cumul": 1.0903 
},
{
 "date":  13056,
"manager": "HAM5",
"perf":  0.007,
"cumul": 1.0979 
},
{
 "date":  13087,
"manager": "HAM5",
"perf": -0.0114,
"cumul": 1.0854 
},
{
 "date":  13117,
"manager": "HAM5",
"perf":  0.023,
"cumul": 1.1104 
},
{
 "date":  13148,
"manager": "HAM5",
"perf": -0.015,
"cumul": 1.0937 
},
{
 "date":  13179,
"manager": "HAM5",
"perf":  0.054,
"cumul": 1.1528 
},
{
 "date":  13207,
"manager": "HAM5",
"perf": -0.0035,
"cumul": 1.1487 
},
{
 "date":  13238,
"manager": "HAM5",
"perf": 0.0362,
"cumul": 1.1903 
},
{
 "date":  13268,
"manager": "HAM5",
"perf": 0.0246,
"cumul": 1.2196 
},
{
 "date":  13299,
"manager": "HAM5",
"perf": -0.0262,
"cumul": 1.1876 
},
{
 "date":  13329,
"manager": "HAM5",
"perf": -0.0114,
"cumul": 1.1741 
},
{
 "date":  13360,
"manager": "HAM5",
"perf": -0.0164,
"cumul": 1.1548 
},
{
 "date":  13391,
"manager": "HAM5",
"perf": 0.0169,
"cumul": 1.1744 
},
{
 "date":  13421,
"manager": "HAM5",
"perf": 0.0132,
"cumul": 1.1899 
},
{
 "date":  13452,
"manager": "HAM5",
"perf": 0.0266,
"cumul": 1.2215 
},
{
 "date":  13482,
"manager": "HAM5",
"perf": 0.0038,
"cumul": 1.2262 
},
{
 "date":  13513,
"manager": "HAM5",
"perf": 0.0317,
"cumul":  1.265 
},
{
 "date":   9526,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9555,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9586,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9616,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9647,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9677,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9708,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9739,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9769,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9800,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9830,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9861,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9892,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9920,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9951,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":   9981,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10012,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10042,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10073,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10104,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10134,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10165,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10195,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10226,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10257,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10285,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10316,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10346,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10377,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10407,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10438,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10469,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10499,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10530,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10560,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10591,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10622,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10650,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10681,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10711,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10742,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10772,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10803,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10834,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10864,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10895,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10925,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10956,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  10987,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11016,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11047,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11077,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11108,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11138,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11169,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11200,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11230,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11261,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11291,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11322,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11353,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11381,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11412,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11442,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11473,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11503,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11534,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11565,
"manager": "HAM6",
"perf": null,
"cumul":      1 
},
{
 "date":  11595,
"manager": "HAM6",
"perf": 0.0023,
"cumul": 1.0023 
},
{
 "date":  11626,
"manager": "HAM6",
"perf": 0.0345,
"cumul": 1.0369 
},
{
 "date":  11656,
"manager": "HAM6",
"perf": 0.0494,
"cumul": 1.0881 
},
{
 "date":  11687,
"manager": "HAM6",
"perf": 0.0501,
"cumul": 1.1426 
},
{
 "date":  11718,
"manager": "HAM6",
"perf": 0.0195,
"cumul": 1.1649 
},
{
 "date":  11746,
"manager": "HAM6",
"perf":  0.013,
"cumul":   1.18 
},
{
 "date":  11777,
"manager": "HAM6",
"perf": 0.0498,
"cumul": 1.2388 
},
{
 "date":  11807,
"manager": "HAM6",
"perf": 0.0047,
"cumul": 1.2446 
},
{
 "date":  11838,
"manager": "HAM6",
"perf": -0.0179,
"cumul": 1.2223 
},
{
 "date":  11868,
"manager": "HAM6",
"perf": -0.0226,
"cumul": 1.1947 
},
{
 "date":  11899,
"manager": "HAM6",
"perf": -0.0403,
"cumul": 1.1466 
},
{
 "date":  11930,
"manager": "HAM6",
"perf": 0.0095,
"cumul": 1.1575 
},
{
 "date":  11960,
"manager": "HAM6",
"perf": 0.0127,
"cumul": 1.1722 
},
{
 "date":  11991,
"manager": "HAM6",
"perf": -0.0091,
"cumul": 1.1615 
},
{
 "date":  12021,
"manager": "HAM6",
"perf": 0.0167,
"cumul": 1.1809 
},
{
 "date":  12052,
"manager": "HAM6",
"perf": -0.0042,
"cumul": 1.1759 
},
{
 "date":  12083,
"manager": "HAM6",
"perf": 0.0017,
"cumul": 1.1779 
},
{
 "date":  12111,
"manager": "HAM6",
"perf": 0.0033,
"cumul": 1.1818 
},
{
 "date":  12142,
"manager": "HAM6",
"perf": 0.0179,
"cumul":  1.203 
},
{
 "date":  12172,
"manager": "HAM6",
"perf": -0.0004,
"cumul": 1.2025 
},
{
 "date":  12203,
"manager": "HAM6",
"perf": 0.0252,
"cumul": 1.2328 
},
{
 "date":  12233,
"manager": "HAM6",
"perf": -0.0007,
"cumul": 1.2319 
},
{
 "date":  12264,
"manager": "HAM6",
"perf": 0.0212,
"cumul": 1.2581 
},
{
 "date":  12295,
"manager": "HAM6",
"perf": 0.0238,
"cumul":  1.288 
},
{
 "date":  12325,
"manager": "HAM6",
"perf": -0.0187,
"cumul": 1.2639 
},
{
 "date":  12356,
"manager": "HAM6",
"perf": 0.0583,
"cumul": 1.3376 
},
{
 "date":  12386,
"manager": "HAM6",
"perf": 0.0102,
"cumul": 1.3512 
},
{
 "date":  12417,
"manager": "HAM6",
"perf":  0.051,
"cumul": 1.4202 
},
{
 "date":  12448,
"manager": "HAM6",
"perf": 0.0252,
"cumul": 1.4559 
},
{
 "date":  12477,
"manager": "HAM6",
"perf": 0.0074,
"cumul": 1.4667 
},
{
 "date":  12508,
"manager": "HAM6",
"perf": 0.0148,
"cumul": 1.4884 
},
{
 "date":  12538,
"manager": "HAM6",
"perf": -0.0187,
"cumul": 1.4606 
},
{
 "date":  12569,
"manager": "HAM6",
"perf": -0.0154,
"cumul": 1.4381 
},
{
 "date":  12599,
"manager": "HAM6",
"perf": 0.0119,
"cumul": 1.4552 
},
{
 "date":  12630,
"manager": "HAM6",
"perf": -0.0361,
"cumul": 1.4027 
},
{
 "date":  12661,
"manager": "HAM6",
"perf": -0.0112,
"cumul":  1.387 
},
{
 "date":  12691,
"manager": "HAM6",
"perf": 0.0189,
"cumul": 1.4132 
},
{
 "date":  12722,
"manager": "HAM6",
"perf": 0.0106,
"cumul": 1.4282 
},
{
 "date":  12752,
"manager": "HAM6",
"perf": 0.0377,
"cumul":  1.482 
},
{
 "date":  12783,
"manager": "HAM6",
"perf": 0.0284,
"cumul": 1.5241 
},
{
 "date":  12814,
"manager": "HAM6",
"perf": -0.014,
"cumul": 1.5028 
},
{
 "date":  12842,
"manager": "HAM6",
"perf": 0.0292,
"cumul": 1.5466 
},
{
 "date":  12873,
"manager": "HAM6",
"perf": -0.0162,
"cumul": 1.5216 
},
{
 "date":  12903,
"manager": "HAM6",
"perf": -0.0401,
"cumul": 1.4606 
},
{
 "date":  12934,
"manager": "HAM6",
"perf": 0.0254,
"cumul": 1.4977 
},
{
 "date":  12964,
"manager": "HAM6",
"perf":  0.012,
"cumul": 1.5156 
},
{
 "date":  12995,
"manager": "HAM6",
"perf": 0.0485,
"cumul": 1.5891 
},
{
 "date":  13026,
"manager": "HAM6",
"perf": 0.0145,
"cumul": 1.6122 
},
{
 "date":  13056,
"manager": "HAM6",
"perf": 0.0257,
"cumul": 1.6536 
},
{
 "date":  13087,
"manager": "HAM6",
"perf": -0.0404,
"cumul": 1.5868 
},
{
 "date":  13117,
"manager": "HAM6",
"perf": 0.0336,
"cumul": 1.6401 
},
{
 "date":  13148,
"manager": "HAM6",
"perf": 0.0261,
"cumul": 1.6829 
},
{
 "date":  13179,
"manager": "HAM6",
"perf": 0.0457,
"cumul": 1.7598 
},
{
 "date":  13207,
"manager": "HAM6",
"perf": 0.0052,
"cumul":  1.769 
},
{
 "date":  13238,
"manager": "HAM6",
"perf": 0.0197,
"cumul": 1.8038 
},
{
 "date":  13268,
"manager": "HAM6",
"perf": 0.0341,
"cumul": 1.8654 
},
{
 "date":  13299,
"manager": "HAM6",
"perf": 0.0075,
"cumul": 1.8793 
},
{
 "date":  13329,
"manager": "HAM6",
"perf": 0.0071,
"cumul": 1.8927 
},
{
 "date":  13360,
"manager": "HAM6",
"perf": -0.0225,
"cumul": 1.8501 
},
{
 "date":  13391,
"manager": "HAM6",
"perf": 0.0193,
"cumul": 1.8858 
},
{
 "date":  13421,
"manager": "HAM6",
"perf": -0.0177,
"cumul": 1.8524 
},
{
 "date":  13452,
"manager": "HAM6",
"perf": 0.0189,
"cumul": 1.8874 
},
{
 "date":  13482,
"manager": "HAM6",
"perf":   0.03,
"cumul": 1.9441 
},
{
 "date":  13513,
"manager": "HAM6",
"perf": 0.0215,
"cumul": 1.9859 
},
{
 "date":   9526,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9555,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9586,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9616,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9647,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9677,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9708,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9739,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9769,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9800,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9830,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9861,
"manager": "EDHEC.LS.EQ",
"perf": null,
"cumul":      1 
},
{
 "date":   9892,
"manager": "EDHEC.LS.EQ",
"perf": 0.0281,
"cumul": 1.0281 
},
{
 "date":   9920,
"manager": "EDHEC.LS.EQ",
"perf": -0.0006,
"cumul": 1.0275 
},
{
 "date":   9951,
"manager": "EDHEC.LS.EQ",
"perf": -0.0084,
"cumul": 1.0189 
},
{
 "date":   9981,
"manager": "EDHEC.LS.EQ",
"perf": 0.0084,
"cumul": 1.0274 
},
{
 "date":  10012,
"manager": "EDHEC.LS.EQ",
"perf": 0.0394,
"cumul": 1.0679 
},
{
 "date":  10042,
"manager": "EDHEC.LS.EQ",
"perf": 0.0223,
"cumul": 1.0917 
},
{
 "date":  10073,
"manager": "EDHEC.LS.EQ",
"perf": 0.0454,
"cumul": 1.1413 
},
{
 "date":  10104,
"manager": "EDHEC.LS.EQ",
"perf": 0.0107,
"cumul": 1.1535 
},
{
 "date":  10134,
"manager": "EDHEC.LS.EQ",
"perf": 0.0429,
"cumul":  1.203 
},
{
 "date":  10165,
"manager": "EDHEC.LS.EQ",
"perf":  0.001,
"cumul": 1.2042 
},
{
 "date":  10195,
"manager": "EDHEC.LS.EQ",
"perf": -0.0026,
"cumul":  1.201 
},
{
 "date":  10226,
"manager": "EDHEC.LS.EQ",
"perf": 0.0104,
"cumul": 1.2135 
},
{
 "date":  10257,
"manager": "EDHEC.LS.EQ",
"perf": 0.0013,
"cumul": 1.2151 
},
{
 "date":  10285,
"manager": "EDHEC.LS.EQ",
"perf": 0.0342,
"cumul": 1.2567 
},
{
 "date":  10316,
"manager": "EDHEC.LS.EQ",
"perf": 0.0336,
"cumul": 1.2989 
},
{
 "date":  10346,
"manager": "EDHEC.LS.EQ",
"perf":  0.012,
"cumul": 1.3145 
},
{
 "date":  10377,
"manager": "EDHEC.LS.EQ",
"perf": -0.0087,
"cumul":  1.303 
},
{
 "date":  10407,
"manager": "EDHEC.LS.EQ",
"perf": 0.0167,
"cumul": 1.3248 
},
{
 "date":  10438,
"manager": "EDHEC.LS.EQ",
"perf": -0.0006,
"cumul":  1.324 
},
{
 "date":  10469,
"manager": "EDHEC.LS.EQ",
"perf": -0.0552,
"cumul": 1.2509 
},
{
 "date":  10499,
"manager": "EDHEC.LS.EQ",
"perf": 0.0206,
"cumul": 1.2767 
},
{
 "date":  10530,
"manager": "EDHEC.LS.EQ",
"perf": 0.0169,
"cumul": 1.2983 
},
{
 "date":  10560,
"manager": "EDHEC.LS.EQ",
"perf": 0.0291,
"cumul":  1.336 
},
{
 "date":  10591,
"manager": "EDHEC.LS.EQ",
"perf": 0.0408,
"cumul": 1.3906 
},
{
 "date":  10622,
"manager": "EDHEC.LS.EQ",
"perf": 0.0258,
"cumul": 1.4264 
},
{
 "date":  10650,
"manager": "EDHEC.LS.EQ",
"perf": -0.0169,
"cumul": 1.4023 
},
{
 "date":  10681,
"manager": "EDHEC.LS.EQ",
"perf": 0.0229,
"cumul": 1.4344 
},
{
 "date":  10711,
"manager": "EDHEC.LS.EQ",
"perf": 0.0312,
"cumul": 1.4792 
},
{
 "date":  10742,
"manager": "EDHEC.LS.EQ",
"perf": 0.0095,
"cumul": 1.4932 
},
{
 "date":  10772,
"manager": "EDHEC.LS.EQ",
"perf": 0.0315,
"cumul": 1.5403 
},
{
 "date":  10803,
"manager": "EDHEC.LS.EQ",
"perf": 0.0177,
"cumul": 1.5675 
},
{
 "date":  10834,
"manager": "EDHEC.LS.EQ",
"perf": 0.0022,
"cumul":  1.571 
},
{
 "date":  10864,
"manager": "EDHEC.LS.EQ",
"perf": 0.0113,
"cumul": 1.5887 
},
{
 "date":  10895,
"manager": "EDHEC.LS.EQ",
"perf": 0.0212,
"cumul": 1.6224 
},
{
 "date":  10925,
"manager": "EDHEC.LS.EQ",
"perf": 0.0481,
"cumul": 1.7005 
},
{
 "date":  10956,
"manager": "EDHEC.LS.EQ",
"perf": 0.0745,
"cumul": 1.8271 
},
{
 "date":  10987,
"manager": "EDHEC.LS.EQ",
"perf": 0.0075,
"cumul": 1.8408 
},
{
 "date":  11016,
"manager": "EDHEC.LS.EQ",
"perf": 0.0699,
"cumul": 1.9695 
},
{
 "date":  11047,
"manager": "EDHEC.LS.EQ",
"perf": 0.0006,
"cumul": 1.9707 
},
{
 "date":  11077,
"manager": "EDHEC.LS.EQ",
"perf": -0.0201,
"cumul": 1.9311 
},
{
 "date":  11108,
"manager": "EDHEC.LS.EQ",
"perf": -0.0097,
"cumul": 1.9124 
},
{
 "date":  11138,
"manager": "EDHEC.LS.EQ",
"perf": 0.0349,
"cumul": 1.9791 
},
{
 "date":  11169,
"manager": "EDHEC.LS.EQ",
"perf": 0.0006,
"cumul": 1.9803 
},
{
 "date":  11200,
"manager": "EDHEC.LS.EQ",
"perf": 0.0345,
"cumul": 2.0486 
},
{
 "date":  11230,
"manager": "EDHEC.LS.EQ",
"perf": -0.0016,
"cumul": 2.0453 
},
{
 "date":  11261,
"manager": "EDHEC.LS.EQ",
"perf": -0.0084,
"cumul": 2.0282 
},
{
 "date":  11291,
"manager": "EDHEC.LS.EQ",
"perf": -0.0153,
"cumul": 1.9971 
},
{
 "date":  11322,
"manager": "EDHEC.LS.EQ",
"perf": 0.0248,
"cumul": 2.0467 
},
{
 "date":  11353,
"manager": "EDHEC.LS.EQ",
"perf": 0.0165,
"cumul": 2.0804 
},
{
 "date":  11381,
"manager": "EDHEC.LS.EQ",
"perf": -0.0264,
"cumul": 2.0255 
},
{
 "date":  11412,
"manager": "EDHEC.LS.EQ",
"perf": -0.0199,
"cumul": 1.9852 
},
{
 "date":  11442,
"manager": "EDHEC.LS.EQ",
"perf": 0.0246,
"cumul":  2.034 
},
{
 "date":  11473,
"manager": "EDHEC.LS.EQ",
"perf": 0.0043,
"cumul": 2.0428 
},
{
 "date":  11503,
"manager": "EDHEC.LS.EQ",
"perf": 0.0019,
"cumul": 2.0467 
},
{
 "date":  11534,
"manager": "EDHEC.LS.EQ",
"perf": -0.0144,
"cumul": 2.0172 
},
{
 "date":  11565,
"manager": "EDHEC.LS.EQ",
"perf": -0.0096,
"cumul": 1.9978 
},
{
 "date":  11595,
"manager": "EDHEC.LS.EQ",
"perf": -0.0348,
"cumul": 1.9283 
},
{
 "date":  11626,
"manager": "EDHEC.LS.EQ",
"perf": 0.0099,
"cumul": 1.9474 
},
{
 "date":  11656,
"manager": "EDHEC.LS.EQ",
"perf":   0.02,
"cumul": 1.9863 
},
{
 "date":  11687,
"manager": "EDHEC.LS.EQ",
"perf":  0.018,
"cumul": 2.0221 
},
{
 "date":  11718,
"manager": "EDHEC.LS.EQ",
"perf": -0.0037,
"cumul": 2.0146 
},
{
 "date":  11746,
"manager": "EDHEC.LS.EQ",
"perf": -0.0123,
"cumul": 1.9898 
},
{
 "date":  11777,
"manager": "EDHEC.LS.EQ",
"perf": 0.0155,
"cumul": 2.0207 
},
{
 "date":  11807,
"manager": "EDHEC.LS.EQ",
"perf": -0.0042,
"cumul": 2.0122 
},
{
 "date":  11838,
"manager": "EDHEC.LS.EQ",
"perf": -0.0034,
"cumul": 2.0053 
},
{
 "date":  11868,
"manager": "EDHEC.LS.EQ",
"perf": -0.0249,
"cumul": 1.9554 
},
{
 "date":  11899,
"manager": "EDHEC.LS.EQ",
"perf": -0.0389,
"cumul": 1.8793 
},
{
 "date":  11930,
"manager": "EDHEC.LS.EQ",
"perf": 0.0041,
"cumul":  1.887 
},
{
 "date":  11960,
"manager": "EDHEC.LS.EQ",
"perf": -0.016,
"cumul": 1.8569 
},
{
 "date":  11991,
"manager": "EDHEC.LS.EQ",
"perf": 0.0123,
"cumul": 1.8797 
},
{
 "date":  12021,
"manager": "EDHEC.LS.EQ",
"perf": 0.0224,
"cumul": 1.9218 
},
{
 "date":  12052,
"manager": "EDHEC.LS.EQ",
"perf": -0.0149,
"cumul": 1.8932 
},
{
 "date":  12083,
"manager": "EDHEC.LS.EQ",
"perf": 0.0005,
"cumul": 1.8941 
},
{
 "date":  12111,
"manager": "EDHEC.LS.EQ",
"perf": -0.0037,
"cumul": 1.8871 
},
{
 "date":  12142,
"manager": "EDHEC.LS.EQ",
"perf":  0.002,
"cumul": 1.8909 
},
{
 "date":  12172,
"manager": "EDHEC.LS.EQ",
"perf": 0.0298,
"cumul": 1.9472 
},
{
 "date":  12203,
"manager": "EDHEC.LS.EQ",
"perf": 0.0362,
"cumul": 2.0177 
},
{
 "date":  12233,
"manager": "EDHEC.LS.EQ",
"perf": 0.0128,
"cumul": 2.0435 
},
{
 "date":  12264,
"manager": "EDHEC.LS.EQ",
"perf": 0.0118,
"cumul": 2.0677 
},
{
 "date":  12295,
"manager": "EDHEC.LS.EQ",
"perf": 0.0179,
"cumul": 2.1047 
},
{
 "date":  12325,
"manager": "EDHEC.LS.EQ",
"perf": 0.0094,
"cumul": 2.1244 
},
{
 "date":  12356,
"manager": "EDHEC.LS.EQ",
"perf": 0.0299,
"cumul":  2.188 
},
{
 "date":  12386,
"manager": "EDHEC.LS.EQ",
"perf":  0.013,
"cumul": 2.2164 
},
{
 "date":  12417,
"manager": "EDHEC.LS.EQ",
"perf": 0.0191,
"cumul": 2.2587 
},
{
 "date":  12448,
"manager": "EDHEC.LS.EQ",
"perf": 0.0192,
"cumul": 2.3021 
},
{
 "date":  12477,
"manager": "EDHEC.LS.EQ",
"perf": 0.0123,
"cumul": 2.3304 
},
{
 "date":  12508,
"manager": "EDHEC.LS.EQ",
"perf": 0.0041,
"cumul":   2.34 
},
{
 "date":  12538,
"manager": "EDHEC.LS.EQ",
"perf": -0.0165,
"cumul": 2.3014 
},
{
 "date":  12569,
"manager": "EDHEC.LS.EQ",
"perf": -0.0035,
"cumul": 2.2933 
},
{
 "date":  12599,
"manager": "EDHEC.LS.EQ",
"perf": 0.0091,
"cumul": 2.3142 
},
{
 "date":  12630,
"manager": "EDHEC.LS.EQ",
"perf": -0.0154,
"cumul": 2.2785 
},
{
 "date":  12661,
"manager": "EDHEC.LS.EQ",
"perf": -0.0022,
"cumul": 2.2735 
},
{
 "date":  12691,
"manager": "EDHEC.LS.EQ",
"perf":  0.021,
"cumul": 2.3213 
},
{
 "date":  12722,
"manager": "EDHEC.LS.EQ",
"perf": 0.0074,
"cumul": 2.3385 
},
{
 "date":  12752,
"manager": "EDHEC.LS.EQ",
"perf": 0.0308,
"cumul": 2.4105 
},
{
 "date":  12783,
"manager": "EDHEC.LS.EQ",
"perf": 0.0178,
"cumul": 2.4534 
},
{
 "date":  12814,
"manager": "EDHEC.LS.EQ",
"perf": -0.0017,
"cumul": 2.4492 
},
{
 "date":  12842,
"manager": "EDHEC.LS.EQ",
"perf":  0.021,
"cumul": 2.5007 
},
{
 "date":  12873,
"manager": "EDHEC.LS.EQ",
"perf": -0.0096,
"cumul": 2.4766 
},
{
 "date":  12903,
"manager": "EDHEC.LS.EQ",
"perf": -0.0184,
"cumul": 2.4311 
},
{
 "date":  12934,
"manager": "EDHEC.LS.EQ",
"perf": 0.0115,
"cumul":  2.459 
},
{
 "date":  12964,
"manager": "EDHEC.LS.EQ",
"perf": 0.0195,
"cumul":  2.507 
},
{
 "date":  12995,
"manager": "EDHEC.LS.EQ",
"perf": 0.0265,
"cumul": 2.5734 
},
{
 "date":  13026,
"manager": "EDHEC.LS.EQ",
"perf": 0.0097,
"cumul": 2.5984 
},
{
 "date":  13056,
"manager": "EDHEC.LS.EQ",
"perf": 0.0222,
"cumul": 2.6561 
},
{
 "date":  13087,
"manager": "EDHEC.LS.EQ",
"perf": -0.0174,
"cumul": 2.6099 
},
{
 "date":  13117,
"manager": "EDHEC.LS.EQ",
"perf": 0.0211,
"cumul": 2.6649 
},
{
 "date":  13148,
"manager": "EDHEC.LS.EQ",
"perf": 0.0249,
"cumul": 2.7313 
},
{
 "date":  13179,
"manager": "EDHEC.LS.EQ",
"perf": 0.0381,
"cumul": 2.8353 
},
{
 "date":  13207,
"manager": "EDHEC.LS.EQ",
"perf": 0.0016,
"cumul": 2.8399 
},
{
 "date":  13238,
"manager": "EDHEC.LS.EQ",
"perf": 0.0238,
"cumul": 2.9075 
},
{
 "date":  13268,
"manager": "EDHEC.LS.EQ",
"perf": 0.0172,
"cumul": 2.9575 
},
{
 "date":  13299,
"manager": "EDHEC.LS.EQ",
"perf": -0.0248,
"cumul": 2.8841 
},
{
 "date":  13329,
"manager": "EDHEC.LS.EQ",
"perf": -0.0062,
"cumul": 2.8662 
},
{
 "date":  13360,
"manager": "EDHEC.LS.EQ",
"perf": -0.0031,
"cumul": 2.8574 
},
{
 "date":  13391,
"manager": "EDHEC.LS.EQ",
"perf": 0.0114,
"cumul": 2.8899 
},
{
 "date":  13421,
"manager": "EDHEC.LS.EQ",
"perf": 0.0001,
"cumul": 2.8902 
},
{
 "date":  13452,
"manager": "EDHEC.LS.EQ",
"perf": 0.0194,
"cumul": 2.9463 
},
{
 "date":  13482,
"manager": "EDHEC.LS.EQ",
"perf":   0.02,
"cumul": 3.0052 
},
{
 "date":  13513,
"manager": "EDHEC.LS.EQ",
"perf": 0.0153,
"cumul": 3.0512 
},
{
 "date":   9526,
"manager": "SP500.TR",
"perf":  0.034,
"cumul":  1.034 
},
{
 "date":   9555,
"manager": "SP500.TR",
"perf": 0.0093,
"cumul": 1.0436 
},
{
 "date":   9586,
"manager": "SP500.TR",
"perf": 0.0096,
"cumul": 1.0536 
},
{
 "date":   9616,
"manager": "SP500.TR",
"perf": 0.0147,
"cumul": 1.0691 
},
{
 "date":   9647,
"manager": "SP500.TR",
"perf": 0.0258,
"cumul": 1.0967 
},
{
 "date":   9677,
"manager": "SP500.TR",
"perf": 0.0038,
"cumul": 1.1009 
},
{
 "date":   9708,
"manager": "SP500.TR",
"perf": -0.0442,
"cumul": 1.0522 
},
{
 "date":   9739,
"manager": "SP500.TR",
"perf": 0.0211,
"cumul": 1.0744 
},
{
 "date":   9769,
"manager": "SP500.TR",
"perf": 0.0563,
"cumul": 1.1349 
},
{
 "date":   9800,
"manager": "SP500.TR",
"perf": 0.0276,
"cumul": 1.1662 
},
{
 "date":   9830,
"manager": "SP500.TR",
"perf": 0.0756,
"cumul": 1.2544 
},
{
 "date":   9861,
"manager": "SP500.TR",
"perf": -0.0198,
"cumul": 1.2296 
},
{
 "date":   9892,
"manager": "SP500.TR",
"perf": 0.0625,
"cumul": 1.3064 
},
{
 "date":   9920,
"manager": "SP500.TR",
"perf": 0.0078,
"cumul": 1.3166 
},
{
 "date":   9951,
"manager": "SP500.TR",
"perf": -0.0411,
"cumul": 1.2625 
},
{
 "date":   9981,
"manager": "SP500.TR",
"perf": 0.0597,
"cumul": 1.3379 
},
{
 "date":  10012,
"manager": "SP500.TR",
"perf": 0.0609,
"cumul": 1.4193 
},
{
 "date":  10042,
"manager": "SP500.TR",
"perf": 0.0448,
"cumul": 1.4829 
},
{
 "date":  10073,
"manager": "SP500.TR",
"perf": 0.0796,
"cumul":  1.601 
},
{
 "date":  10104,
"manager": "SP500.TR",
"perf": -0.056,
"cumul": 1.5113 
},
{
 "date":  10134,
"manager": "SP500.TR",
"perf": 0.0548,
"cumul": 1.5941 
},
{
 "date":  10165,
"manager": "SP500.TR",
"perf": -0.0334,
"cumul": 1.5409 
},
{
 "date":  10195,
"manager": "SP500.TR",
"perf": 0.0463,
"cumul": 1.6122 
},
{
 "date":  10226,
"manager": "SP500.TR",
"perf": 0.0172,
"cumul":   1.64 
},
{
 "date":  10257,
"manager": "SP500.TR",
"perf": 0.0111,
"cumul": 1.6582 
},
{
 "date":  10285,
"manager": "SP500.TR",
"perf": 0.0721,
"cumul": 1.7777 
},
{
 "date":  10316,
"manager": "SP500.TR",
"perf": 0.0512,
"cumul": 1.8687 
},
{
 "date":  10346,
"manager": "SP500.TR",
"perf": 0.0101,
"cumul": 1.8876 
},
{
 "date":  10377,
"manager": "SP500.TR",
"perf": -0.0172,
"cumul": 1.8551 
},
{
 "date":  10407,
"manager": "SP500.TR",
"perf": 0.0406,
"cumul": 1.9305 
},
{
 "date":  10438,
"manager": "SP500.TR",
"perf": -0.0106,
"cumul":   1.91 
},
{
 "date":  10469,
"manager": "SP500.TR",
"perf": -0.1446,
"cumul": 1.6338 
},
{
 "date":  10499,
"manager": "SP500.TR",
"perf": 0.0641,
"cumul": 1.7385 
},
{
 "date":  10530,
"manager": "SP500.TR",
"perf": 0.0813,
"cumul": 1.8799 
},
{
 "date":  10560,
"manager": "SP500.TR",
"perf": 0.0606,
"cumul": 1.9938 
},
{
 "date":  10591,
"manager": "SP500.TR",
"perf": 0.0576,
"cumul": 2.1086 
},
{
 "date":  10622,
"manager": "SP500.TR",
"perf": 0.0418,
"cumul": 2.1968 
},
{
 "date":  10650,
"manager": "SP500.TR",
"perf": -0.0311,
"cumul": 2.1285 
},
{
 "date":  10681,
"manager": "SP500.TR",
"perf":   0.04,
"cumul": 2.2136 
},
{
 "date":  10711,
"manager": "SP500.TR",
"perf": 0.0387,
"cumul": 2.2993 
},
{
 "date":  10742,
"manager": "SP500.TR",
"perf": -0.0236,
"cumul":  2.245 
},
{
 "date":  10772,
"manager": "SP500.TR",
"perf": 0.0555,
"cumul": 2.3696 
},
{
 "date":  10803,
"manager": "SP500.TR",
"perf": -0.0312,
"cumul": 2.2957 
},
{
 "date":  10834,
"manager": "SP500.TR",
"perf": -0.0049,
"cumul": 2.2844 
},
{
 "date":  10864,
"manager": "SP500.TR",
"perf": -0.0274,
"cumul": 2.2218 
},
{
 "date":  10895,
"manager": "SP500.TR",
"perf": 0.0633,
"cumul": 2.3625 
},
{
 "date":  10925,
"manager": "SP500.TR",
"perf": 0.0203,
"cumul": 2.4104 
},
{
 "date":  10956,
"manager": "SP500.TR",
"perf": 0.0589,
"cumul": 2.5524 
},
{
 "date":  10987,
"manager": "SP500.TR",
"perf": -0.0502,
"cumul": 2.4243 
},
{
 "date":  11016,
"manager": "SP500.TR",
"perf": -0.0189,
"cumul": 2.3785 
},
{
 "date":  11047,
"manager": "SP500.TR",
"perf": 0.0978,
"cumul": 2.6111 
},
{
 "date":  11077,
"manager": "SP500.TR",
"perf": -0.0301,
"cumul": 2.5325 
},
{
 "date":  11108,
"manager": "SP500.TR",
"perf": -0.0205,
"cumul": 2.4806 
},
{
 "date":  11138,
"manager": "SP500.TR",
"perf": 0.0247,
"cumul": 2.5418 
},
{
 "date":  11169,
"manager": "SP500.TR",
"perf": -0.0156,
"cumul": 2.5022 
},
{
 "date":  11200,
"manager": "SP500.TR",
"perf": 0.0621,
"cumul": 2.6576 
},
{
 "date":  11230,
"manager": "SP500.TR",
"perf": -0.0528,
"cumul": 2.5172 
},
{
 "date":  11261,
"manager": "SP500.TR",
"perf": -0.0042,
"cumul": 2.5067 
},
{
 "date":  11291,
"manager": "SP500.TR",
"perf": -0.0788,
"cumul": 2.3091 
},
{
 "date":  11322,
"manager": "SP500.TR",
"perf": 0.0049,
"cumul": 2.3205 
},
{
 "date":  11353,
"manager": "SP500.TR",
"perf": 0.0355,
"cumul": 2.4028 
},
{
 "date":  11381,
"manager": "SP500.TR",
"perf": -0.0912,
"cumul": 2.1837 
},
{
 "date":  11412,
"manager": "SP500.TR",
"perf": -0.0634,
"cumul": 2.0452 
},
{
 "date":  11442,
"manager": "SP500.TR",
"perf": 0.0777,
"cumul": 2.2042 
},
{
 "date":  11473,
"manager": "SP500.TR",
"perf": 0.0067,
"cumul": 2.2189 
},
{
 "date":  11503,
"manager": "SP500.TR",
"perf": -0.0243,
"cumul":  2.165 
},
{
 "date":  11534,
"manager": "SP500.TR",
"perf": -0.0098,
"cumul": 2.1438 
},
{
 "date":  11565,
"manager": "SP500.TR",
"perf": -0.0626,
"cumul": 2.0096 
},
{
 "date":  11595,
"manager": "SP500.TR",
"perf": -0.0808,
"cumul": 1.8472 
},
{
 "date":  11626,
"manager": "SP500.TR",
"perf": 0.0191,
"cumul": 1.8825 
},
{
 "date":  11656,
"manager": "SP500.TR",
"perf": 0.0767,
"cumul": 2.0269 
},
{
 "date":  11687,
"manager": "SP500.TR",
"perf": 0.0088,
"cumul": 2.0447 
},
{
 "date":  11718,
"manager": "SP500.TR",
"perf": -0.0146,
"cumul": 2.0149 
},
{
 "date":  11746,
"manager": "SP500.TR",
"perf": -0.0193,
"cumul":  1.976 
},
{
 "date":  11777,
"manager": "SP500.TR",
"perf": 0.0376,
"cumul": 2.0503 
},
{
 "date":  11807,
"manager": "SP500.TR",
"perf": -0.0606,
"cumul":  1.926 
},
{
 "date":  11838,
"manager": "SP500.TR",
"perf": -0.0074,
"cumul": 1.9118 
},
{
 "date":  11868,
"manager": "SP500.TR",
"perf": -0.0712,
"cumul": 1.7757 
},
{
 "date":  11899,
"manager": "SP500.TR",
"perf": -0.078,
"cumul": 1.6372 
},
{
 "date":  11930,
"manager": "SP500.TR",
"perf": 0.0066,
"cumul":  1.648 
},
{
 "date":  11960,
"manager": "SP500.TR",
"perf": -0.1087,
"cumul": 1.4688 
},
{
 "date":  11991,
"manager": "SP500.TR",
"perf":  0.088,
"cumul": 1.5981 
},
{
 "date":  12021,
"manager": "SP500.TR",
"perf": 0.0589,
"cumul": 1.6922 
},
{
 "date":  12052,
"manager": "SP500.TR",
"perf": -0.0587,
"cumul": 1.5929 
},
{
 "date":  12083,
"manager": "SP500.TR",
"perf": -0.0262,
"cumul": 1.5511 
},
{
 "date":  12111,
"manager": "SP500.TR",
"perf": -0.015,
"cumul": 1.5279 
},
{
 "date":  12142,
"manager": "SP500.TR",
"perf": 0.0097,
"cumul": 1.5427 
},
{
 "date":  12172,
"manager": "SP500.TR",
"perf": 0.0824,
"cumul": 1.6698 
},
{
 "date":  12203,
"manager": "SP500.TR",
"perf": 0.0527,
"cumul": 1.7578 
},
{
 "date":  12233,
"manager": "SP500.TR",
"perf": 0.0128,
"cumul": 1.7803 
},
{
 "date":  12264,
"manager": "SP500.TR",
"perf": 0.0176,
"cumul": 1.8117 
},
{
 "date":  12295,
"manager": "SP500.TR",
"perf": 0.0195,
"cumul":  1.847 
},
{
 "date":  12325,
"manager": "SP500.TR",
"perf": -0.0106,
"cumul": 1.8274 
},
{
 "date":  12356,
"manager": "SP500.TR",
"perf": 0.0566,
"cumul": 1.9308 
},
{
 "date":  12386,
"manager": "SP500.TR",
"perf": 0.0088,
"cumul": 1.9478 
},
{
 "date":  12417,
"manager": "SP500.TR",
"perf": 0.0524,
"cumul": 2.0499 
},
{
 "date":  12448,
"manager": "SP500.TR",
"perf": 0.0184,
"cumul": 2.0876 
},
{
 "date":  12477,
"manager": "SP500.TR",
"perf": 0.0139,
"cumul": 2.1166 
},
{
 "date":  12508,
"manager": "SP500.TR",
"perf": -0.0151,
"cumul": 2.0847 
},
{
 "date":  12538,
"manager": "SP500.TR",
"perf": -0.0157,
"cumul": 2.0519 
},
{
 "date":  12569,
"manager": "SP500.TR",
"perf": 0.0137,
"cumul": 2.0801 
},
{
 "date":  12599,
"manager": "SP500.TR",
"perf": 0.0195,
"cumul": 2.1206 
},
{
 "date":  12630,
"manager": "SP500.TR",
"perf": -0.0331,
"cumul": 2.0504 
},
{
 "date":  12661,
"manager": "SP500.TR",
"perf": 0.0041,
"cumul": 2.0588 
},
{
 "date":  12691,
"manager": "SP500.TR",
"perf": 0.0108,
"cumul": 2.0811 
},
{
 "date":  12722,
"manager": "SP500.TR",
"perf": 0.0153,
"cumul": 2.1129 
},
{
 "date":  12752,
"manager": "SP500.TR",
"perf": 0.0405,
"cumul": 2.1985 
},
{
 "date":  12783,
"manager": "SP500.TR",
"perf":  0.034,
"cumul": 2.2732 
},
{
 "date":  12814,
"manager": "SP500.TR",
"perf": -0.024375,
"cumul": 2.2178 
},
{
 "date":  12842,
"manager": "SP500.TR",
"perf": 0.02104,
"cumul": 2.2645 
},
{
 "date":  12873,
"manager": "SP500.TR",
"perf": -0.01771,
"cumul": 2.2244 
},
{
 "date":  12903,
"manager": "SP500.TR",
"perf": -0.019,
"cumul": 2.1821 
},
{
 "date":  12934,
"manager": "SP500.TR",
"perf": 0.03182,
"cumul": 2.2515 
},
{
 "date":  12964,
"manager": "SP500.TR",
"perf": 0.00142,
"cumul": 2.2547 
},
{
 "date":  12995,
"manager": "SP500.TR",
"perf": 0.0372,
"cumul": 2.3386 
},
{
 "date":  13026,
"manager": "SP500.TR",
"perf": -0.0091,
"cumul": 2.3173 
},
{
 "date":  13056,
"manager": "SP500.TR",
"perf": 0.0081,
"cumul": 2.3361 
},
{
 "date":  13087,
"manager": "SP500.TR",
"perf": -0.0167,
"cumul": 2.2971 
},
{
 "date":  13117,
"manager": "SP500.TR",
"perf": 0.0378,
"cumul": 2.3839 
},
{
 "date":  13148,
"manager": "SP500.TR",
"perf": 0.0003,
"cumul": 2.3846 
},
{
 "date":  13179,
"manager": "SP500.TR",
"perf": 0.0265,
"cumul": 2.4478 
},
{
 "date":  13207,
"manager": "SP500.TR",
"perf": 0.0027,
"cumul": 2.4544 
},
{
 "date":  13238,
"manager": "SP500.TR",
"perf": 0.0125,
"cumul": 2.4851 
},
{
 "date":  13268,
"manager": "SP500.TR",
"perf": 0.0134,
"cumul": 2.5184 
},
{
 "date":  13299,
"manager": "SP500.TR",
"perf": -0.0288,
"cumul": 2.4459 
},
{
 "date":  13329,
"manager": "SP500.TR",
"perf": 0.0014,
"cumul": 2.4493 
},
{
 "date":  13360,
"manager": "SP500.TR",
"perf": 0.0062,
"cumul": 2.4645 
},
{
 "date":  13391,
"manager": "SP500.TR",
"perf": 0.0238,
"cumul": 2.5232 
},
{
 "date":  13421,
"manager": "SP500.TR",
"perf": 0.0258,
"cumul": 2.5883 
},
{
 "date":  13452,
"manager": "SP500.TR",
"perf": 0.0326,
"cumul": 2.6726 
},
{
 "date":  13482,
"manager": "SP500.TR",
"perf":  0.019,
"cumul": 2.7234 
},
{
 "date":  13513,
"manager": "SP500.TR",
"perf": 0.01403,
"cumul": 2.7616 
},
{
 "date":   9526,
"manager": "US.10Y.TR",
"perf": 0.0038,
"cumul": 1.0038 
},
{
 "date":   9555,
"manager": "US.10Y.TR",
"perf": -0.03532,
"cumul": 0.96835 
},
{
 "date":   9586,
"manager": "US.10Y.TR",
"perf": -0.01057,
"cumul": 0.95811 
},
{
 "date":   9616,
"manager": "US.10Y.TR",
"perf": -0.01739,
"cumul": 0.94145 
},
{
 "date":   9647,
"manager": "US.10Y.TR",
"perf": -0.00543,
"cumul": 0.93634 
},
{
 "date":   9677,
"manager": "US.10Y.TR",
"perf": 0.01507,
"cumul": 0.95045 
},
{
 "date":   9708,
"manager": "US.10Y.TR",
"perf": -0.001,
"cumul": 0.9495 
},
{
 "date":   9739,
"manager": "US.10Y.TR",
"perf": -0.00448,
"cumul": 0.94524 
},
{
 "date":   9769,
"manager": "US.10Y.TR",
"perf": 0.02229,
"cumul": 0.96631 
},
{
 "date":   9800,
"manager": "US.10Y.TR",
"perf": 0.02869,
"cumul": 0.99404 
},
{
 "date":   9830,
"manager": "US.10Y.TR",
"perf": 0.02797,
"cumul": 1.0218 
},
{
 "date":   9861,
"manager": "US.10Y.TR",
"perf": -0.02094,
"cumul": 1.0004 
},
{
 "date":   9892,
"manager": "US.10Y.TR",
"perf": -0.00055,
"cumul": 0.99989 
},
{
 "date":   9920,
"manager": "US.10Y.TR",
"perf": -0.00167,
"cumul": 0.99822 
},
{
 "date":   9951,
"manager": "US.10Y.TR",
"perf": -0.01958,
"cumul": 0.97868 
},
{
 "date":   9981,
"manager": "US.10Y.TR",
"perf": 0.01954,
"cumul": 0.9978 
},
{
 "date":  10012,
"manager": "US.10Y.TR",
"perf": 0.01033,
"cumul": 1.0081 
},
{
 "date":  10042,
"manager": "US.10Y.TR",
"perf": 0.01665,
"cumul": 1.0249 
},
{
 "date":  10073,
"manager": "US.10Y.TR",
"perf": 0.04161,
"cumul": 1.0675 
},
{
 "date":  10104,
"manager": "US.10Y.TR",
"perf": -0.02148,
"cumul": 1.0446 
},
{
 "date":  10134,
"manager": "US.10Y.TR",
"perf": 0.02153,
"cumul": 1.0671 
},
{
 "date":  10165,
"manager": "US.10Y.TR",
"perf": 0.0262,
"cumul": 1.0951 
},
{
 "date":  10195,
"manager": "US.10Y.TR",
"perf": 0.00241,
"cumul": 1.0977 
},
{
 "date":  10226,
"manager": "US.10Y.TR",
"perf": 0.01311,
"cumul": 1.1121 
},
{
 "date":  10257,
"manager": "US.10Y.TR",
"perf": 0.02067,
"cumul": 1.1351 
},
{
 "date":  10285,
"manager": "US.10Y.TR",
"perf": -0.00846,
"cumul": 1.1255 
},
{
 "date":  10316,
"manager": "US.10Y.TR",
"perf": 0.00159,
"cumul": 1.1273 
},
{
 "date":  10346,
"manager": "US.10Y.TR",
"perf": 0.00333,
"cumul":  1.131 
},
{
 "date":  10377,
"manager": "US.10Y.TR",
"perf": 0.01102,
"cumul": 1.1435 
},
{
 "date":  10407,
"manager": "US.10Y.TR",
"perf": 0.01324,
"cumul": 1.1586 
},
{
 "date":  10438,
"manager": "US.10Y.TR",
"perf": 0.00051,
"cumul": 1.1592 
},
{
 "date":  10469,
"manager": "US.10Y.TR",
"perf": 0.03923,
"cumul": 1.2047 
},
{
 "date":  10499,
"manager": "US.10Y.TR",
"perf": 0.05055,
"cumul": 1.2656 
},
{
 "date":  10530,
"manager": "US.10Y.TR",
"perf": -0.00991,
"cumul":  1.253 
},
{
 "date":  10560,
"manager": "US.10Y.TR",
"perf": -0.00937,
"cumul": 1.2413 
},
{
 "date":  10591,
"manager": "US.10Y.TR",
"perf": 0.01028,
"cumul": 1.2541 
},
{
 "date":  10622,
"manager": "US.10Y.TR",
"perf": 0.00417,
"cumul": 1.2593 
},
{
 "date":  10650,
"manager": "US.10Y.TR",
"perf": -0.04474,
"cumul": 1.2029 
},
{
 "date":  10681,
"manager": "US.10Y.TR",
"perf": 0.00884,
"cumul": 1.2136 
},
{
 "date":  10711,
"manager": "US.10Y.TR",
"perf": -0.00427,
"cumul": 1.2084 
},
{
 "date":  10742,
"manager": "US.10Y.TR",
"perf": -0.01909,
"cumul": 1.1853 
},
{
 "date":  10772,
"manager": "US.10Y.TR",
"perf": -0.00933,
"cumul": 1.1743 
},
{
 "date":  10803,
"manager": "US.10Y.TR",
"perf": -0.00227,
"cumul": 1.1716 
},
{
 "date":  10834,
"manager": "US.10Y.TR",
"perf": -0.00516,
"cumul": 1.1656 
},
{
 "date":  10864,
"manager": "US.10Y.TR",
"perf": 0.01128,
"cumul": 1.1787 
},
{
 "date":  10895,
"manager": "US.10Y.TR",
"perf": -0.00487,
"cumul":  1.173 
},
{
 "date":  10925,
"manager": "US.10Y.TR",
"perf": -0.00571,
"cumul": 1.1663 
},
{
 "date":  10956,
"manager": "US.10Y.TR",
"perf": -0.01347,
"cumul": 1.1506 
},
{
 "date":  10987,
"manager": "US.10Y.TR",
"perf": -0.01067,
"cumul": 1.1383 
},
{
 "date":  11016,
"manager": "US.10Y.TR",
"perf": 0.01669,
"cumul": 1.1573 
},
{
 "date":  11047,
"manager": "US.10Y.TR",
"perf": 0.03431,
"cumul":  1.197 
},
{
 "date":  11077,
"manager": "US.10Y.TR",
"perf": -0.0094,
"cumul": 1.1857 
},
{
 "date":  11108,
"manager": "US.10Y.TR",
"perf": 0.00037,
"cumul": 1.1862 
},
{
 "date":  11138,
"manager": "US.10Y.TR",
"perf": 0.02408,
"cumul": 1.2147 
},
{
 "date":  11169,
"manager": "US.10Y.TR",
"perf": 0.00405,
"cumul": 1.2197 
},
{
 "date":  11200,
"manager": "US.10Y.TR",
"perf": 0.01644,
"cumul": 1.2397 
},
{
 "date":  11230,
"manager": "US.10Y.TR",
"perf": -0.00015,
"cumul": 1.2395 
},
{
 "date":  11261,
"manager": "US.10Y.TR",
"perf": 0.00794,
"cumul": 1.2494 
},
{
 "date":  11291,
"manager": "US.10Y.TR",
"perf": 0.0272,
"cumul": 1.2833 
},
{
 "date":  11322,
"manager": "US.10Y.TR",
"perf": 0.02979,
"cumul": 1.3216 
},
{
 "date":  11353,
"manager": "US.10Y.TR",
"perf": 0.00102,
"cumul": 1.3229 
},
{
 "date":  11381,
"manager": "US.10Y.TR",
"perf": 0.01458,
"cumul": 1.3422 
},
{
 "date":  11412,
"manager": "US.10Y.TR",
"perf": 0.00287,
"cumul": 1.3461 
},
{
 "date":  11442,
"manager": "US.10Y.TR",
"perf": -0.02603,
"cumul":  1.311 
},
{
 "date":  11473,
"manager": "US.10Y.TR",
"perf": -0.00073,
"cumul": 1.3101 
},
{
 "date":  11503,
"manager": "US.10Y.TR",
"perf": 0.00468,
"cumul": 1.3162 
},
{
 "date":  11534,
"manager": "US.10Y.TR",
"perf": 0.03152,
"cumul": 1.3577 
},
{
 "date":  11565,
"manager": "US.10Y.TR",
"perf": 0.01534,
"cumul": 1.3785 
},
{
 "date":  11595,
"manager": "US.10Y.TR",
"perf": 0.02277,
"cumul": 1.4099 
},
{
 "date":  11626,
"manager": "US.10Y.TR",
"perf": 0.02796,
"cumul": 1.4493 
},
{
 "date":  11656,
"manager": "US.10Y.TR",
"perf": -0.03231,
"cumul": 1.4025 
},
{
 "date":  11687,
"manager": "US.10Y.TR",
"perf": -0.01755,
"cumul": 1.3779 
},
{
 "date":  11718,
"manager": "US.10Y.TR",
"perf": 0.00493,
"cumul": 1.3847 
},
{
 "date":  11746,
"manager": "US.10Y.TR",
"perf": 0.01281,
"cumul": 1.4024 
},
{
 "date":  11777,
"manager": "US.10Y.TR",
"perf": -0.03714,
"cumul": 1.3503 
},
{
 "date":  11807,
"manager": "US.10Y.TR",
"perf": 0.02863,
"cumul":  1.389 
},
{
 "date":  11838,
"manager": "US.10Y.TR",
"perf": 0.00844,
"cumul": 1.4007 
},
{
 "date":  11868,
"manager": "US.10Y.TR",
"perf": 0.02058,
"cumul": 1.4295 
},
{
 "date":  11899,
"manager": "US.10Y.TR",
"perf": 0.03138,
"cumul": 1.4744 
},
{
 "date":  11930,
"manager": "US.10Y.TR",
"perf": 0.02985,
"cumul": 1.5184 
},
{
 "date":  11960,
"manager": "US.10Y.TR",
"perf": 0.04685,
"cumul": 1.5895 
},
{
 "date":  11991,
"manager": "US.10Y.TR",
"perf": -0.02009,
"cumul": 1.5576 
},
{
 "date":  12021,
"manager": "US.10Y.TR",
"perf": -0.02073,
"cumul": 1.5253 
},
{
 "date":  12052,
"manager": "US.10Y.TR",
"perf": 0.0354,
"cumul": 1.5793 
},
{
 "date":  12083,
"manager": "US.10Y.TR",
"perf": -0.00868,
"cumul": 1.5656 
},
{
 "date":  12111,
"manager": "US.10Y.TR",
"perf": 0.02766,
"cumul": 1.6089 
},
{
 "date":  12142,
"manager": "US.10Y.TR",
"perf": -0.00711,
"cumul": 1.5975 
},
{
 "date":  12172,
"manager": "US.10Y.TR",
"perf": 0.00035,
"cumul":  1.598 
},
{
 "date":  12203,
"manager": "US.10Y.TR",
"perf": 0.04658,
"cumul": 1.6725 
},
{
 "date":  12233,
"manager": "US.10Y.TR",
"perf": -0.01184,
"cumul": 1.6527 
},
{
 "date":  12264,
"manager": "US.10Y.TR",
"perf": -0.07092,
"cumul": 1.5355 
},
{
 "date":  12295,
"manager": "US.10Y.TR",
"perf": 0.01076,
"cumul":  1.552 
},
{
 "date":  12325,
"manager": "US.10Y.TR",
"perf": 0.04548,
"cumul": 1.6226 
},
{
 "date":  12356,
"manager": "US.10Y.TR",
"perf": -0.02484,
"cumul": 1.5823 
},
{
 "date":  12386,
"manager": "US.10Y.TR",
"perf": 0.00293,
"cumul": 1.5869 
},
{
 "date":  12417,
"manager": "US.10Y.TR",
"perf": 0.00834,
"cumul": 1.6001 
},
{
 "date":  12448,
"manager": "US.10Y.TR",
"perf": 0.01372,
"cumul": 1.6221 
},
{
 "date":  12477,
"manager": "US.10Y.TR",
"perf": 0.01671,
"cumul": 1.6492 
},
{
 "date":  12508,
"manager": "US.10Y.TR",
"perf": 0.01523,
"cumul": 1.6743 
},
{
 "date":  12538,
"manager": "US.10Y.TR",
"perf": -0.04833,
"cumul": 1.5934 
},
{
 "date":  12569,
"manager": "US.10Y.TR",
"perf": -0.00681,
"cumul": 1.5825 
},
{
 "date":  12599,
"manager": "US.10Y.TR",
"perf": 0.00674,
"cumul": 1.5932 
},
{
 "date":  12630,
"manager": "US.10Y.TR",
"perf": 0.01477,
"cumul": 1.6167 
},
{
 "date":  12661,
"manager": "US.10Y.TR",
"perf": 0.03108,
"cumul":  1.667 
},
{
 "date":  12691,
"manager": "US.10Y.TR",
"perf": 0.00388,
"cumul": 1.6735 
},
{
 "date":  12722,
"manager": "US.10Y.TR",
"perf": 0.0106,
"cumul": 1.6912 
},
{
 "date":  12752,
"manager": "US.10Y.TR",
"perf": -0.02276,
"cumul": 1.6527 
},
{
 "date":  12783,
"manager": "US.10Y.TR",
"perf": 0.01495,
"cumul": 1.6774 
},
{
 "date":  12814,
"manager": "US.10Y.TR",
"perf": 0.01016,
"cumul": 1.6945 
},
{
 "date":  12842,
"manager": "US.10Y.TR",
"perf": -0.01518,
"cumul": 1.6687 
},
{
 "date":  12873,
"manager": "US.10Y.TR",
"perf": -0.00724,
"cumul": 1.6566 
},
{
 "date":  12903,
"manager": "US.10Y.TR",
"perf": 0.02725,
"cumul": 1.7018 
},
{
 "date":  12934,
"manager": "US.10Y.TR",
"perf": 0.01744,
"cumul": 1.7315 
},
{
 "date":  12964,
"manager": "US.10Y.TR",
"perf": 0.00819,
"cumul": 1.7457 
},
{
 "date":  12995,
"manager": "US.10Y.TR",
"perf": -0.02332,
"cumul": 1.7049 
},
{
 "date":  13026,
"manager": "US.10Y.TR",
"perf": 0.02267,
"cumul": 1.7436 
},
{
 "date":  13056,
"manager": "US.10Y.TR",
"perf": -0.02124,
"cumul": 1.7066 
},
{
 "date":  13087,
"manager": "US.10Y.TR",
"perf": -0.0144,
"cumul":  1.682 
},
{
 "date":  13117,
"manager": "US.10Y.TR",
"perf": 0.00518,
"cumul": 1.6907 
},
{
 "date":  13148,
"manager": "US.10Y.TR",
"perf": 0.01188,
"cumul": 1.7108 
},
{
 "date":  13179,
"manager": "US.10Y.TR",
"perf": -0.00657,
"cumul": 1.6995 
},
{
 "date":  13207,
"manager": "US.10Y.TR",
"perf": -0.00139,
"cumul": 1.6972 
},
{
 "date":  13238,
"manager": "US.10Y.TR",
"perf": -0.01987,
"cumul": 1.6635 
},
{
 "date":  13268,
"manager": "US.10Y.TR",
"perf": -0.01272,
"cumul": 1.6423 
},
{
 "date":  13299,
"manager": "US.10Y.TR",
"perf": -0.00082,
"cumul":  1.641 
},
{
 "date":  13329,
"manager": "US.10Y.TR",
"perf": 0.00221,
"cumul": 1.6446 
},
{
 "date":  13360,
"manager": "US.10Y.TR",
"perf": 0.0158,
"cumul": 1.6706 
},
{
 "date":  13391,
"manager": "US.10Y.TR",
"perf": 0.0219,
"cumul": 1.7071 
},
{
 "date":  13421,
"manager": "US.10Y.TR",
"perf": 0.0114,
"cumul": 1.7266 
},
{
 "date":  13452,
"manager": "US.10Y.TR",
"perf": 0.00584,
"cumul": 1.7367 
},
{
 "date":  13482,
"manager": "US.10Y.TR",
"perf": 0.01419,
"cumul": 1.7613 
},
{
 "date":  13513,
"manager": "US.10Y.TR",
"perf": -0.0155,
"cumul":  1.734 
},
{
 "date":   9526,
"manager": "US.3m.TR",
"perf": 0.00456,
"cumul": 1.0046 
},
{
 "date":   9555,
"manager": "US.3m.TR",
"perf": 0.00398,
"cumul": 1.0086 
},
{
 "date":   9586,
"manager": "US.3m.TR",
"perf": 0.00371,
"cumul": 1.0123 
},
{
 "date":   9616,
"manager": "US.3m.TR",
"perf": 0.00428,
"cumul": 1.0166 
},
{
 "date":   9647,
"manager": "US.3m.TR",
"perf": 0.00443,
"cumul": 1.0211 
},
{
 "date":   9677,
"manager": "US.3m.TR",
"perf": 0.00412,
"cumul": 1.0253 
},
{
 "date":   9708,
"manager": "US.3m.TR",
"perf": 0.00454,
"cumul":   1.03 
},
{
 "date":   9739,
"manager": "US.3m.TR",
"perf": 0.00451,
"cumul": 1.0346 
},
{
 "date":   9769,
"manager": "US.3m.TR",
"perf": 0.0047,
"cumul": 1.0395 
},
{
 "date":   9800,
"manager": "US.3m.TR",
"perf": 0.00428,
"cumul":  1.044 
},
{
 "date":   9830,
"manager": "US.3m.TR",
"perf": 0.00427,
"cumul": 1.0484 
},
{
 "date":   9861,
"manager": "US.3m.TR",
"perf": 0.00442,
"cumul":  1.053 
},
{
 "date":   9892,
"manager": "US.3m.TR",
"perf": 0.00457,
"cumul": 1.0579 
},
{
 "date":   9920,
"manager": "US.3m.TR",
"perf": 0.0039,
"cumul":  1.062 
},
{
 "date":   9951,
"manager": "US.3m.TR",
"perf": 0.00422,
"cumul": 1.0665 
},
{
 "date":   9981,
"manager": "US.3m.TR",
"perf": 0.00477,
"cumul": 1.0716 
},
{
 "date":  10012,
"manager": "US.3m.TR",
"perf": 0.00513,
"cumul": 1.0771 
},
{
 "date":  10042,
"manager": "US.3m.TR",
"perf": 0.00365,
"cumul":  1.081 
},
{
 "date":  10073,
"manager": "US.3m.TR",
"perf": 0.0045,
"cumul": 1.0858 
},
{
 "date":  10104,
"manager": "US.3m.TR",
"perf": 0.00428,
"cumul": 1.0905 
},
{
 "date":  10134,
"manager": "US.3m.TR",
"perf": 0.00458,
"cumul": 1.0955 
},
{
 "date":  10165,
"manager": "US.3m.TR",
"perf": 0.00427,
"cumul": 1.1002 
},
{
 "date":  10195,
"manager": "US.3m.TR",
"perf": 0.0039,
"cumul": 1.1045 
},
{
 "date":  10226,
"manager": "US.3m.TR",
"perf": 0.00429,
"cumul": 1.1092 
},
{
 "date":  10257,
"manager": "US.3m.TR",
"perf": 0.00468,
"cumul": 1.1144 
},
{
 "date":  10285,
"manager": "US.3m.TR",
"perf": 0.00355,
"cumul": 1.1183 
},
{
 "date":  10316,
"manager": "US.3m.TR",
"perf": 0.00473,
"cumul": 1.1236 
},
{
 "date":  10346,
"manager": "US.3m.TR",
"perf": 0.00449,
"cumul": 1.1287 
},
{
 "date":  10377,
"manager": "US.3m.TR",
"perf": 0.00416,
"cumul": 1.1334 
},
{
 "date":  10407,
"manager": "US.3m.TR",
"perf": 0.00419,
"cumul": 1.1381 
},
{
 "date":  10438,
"manager": "US.3m.TR",
"perf": 0.00443,
"cumul": 1.1432 
},
{
 "date":  10469,
"manager": "US.3m.TR",
"perf": 0.00456,
"cumul": 1.1484 
},
{
 "date":  10499,
"manager": "US.3m.TR",
"perf": 0.00511,
"cumul": 1.1542 
},
{
 "date":  10530,
"manager": "US.3m.TR",
"perf": 0.00393,
"cumul": 1.1588 
},
{
 "date":  10560,
"manager": "US.3m.TR",
"perf": 0.00333,
"cumul": 1.1626 
},
{
 "date":  10591,
"manager": "US.3m.TR",
"perf": 0.00395,
"cumul": 1.1672 
},
{
 "date":  10622,
"manager": "US.3m.TR",
"perf": 0.00355,
"cumul": 1.1714 
},
{
 "date":  10650,
"manager": "US.3m.TR",
"perf": 0.00287,
"cumul": 1.1747 
},
{
 "date":  10681,
"manager": "US.3m.TR",
"perf": 0.00411,
"cumul": 1.1796 
},
{
 "date":  10711,
"manager": "US.3m.TR",
"perf": 0.00385,
"cumul": 1.1841 
},
{
 "date":  10742,
"manager": "US.3m.TR",
"perf": 0.00389,
"cumul": 1.1887 
},
{
 "date":  10772,
"manager": "US.3m.TR",
"perf": 0.00418,
"cumul": 1.1937 
},
{
 "date":  10803,
"manager": "US.3m.TR",
"perf": 0.00408,
"cumul": 1.1986 
},
{
 "date":  10834,
"manager": "US.3m.TR",
"perf": 0.00402,
"cumul": 1.2034 
},
{
 "date":  10864,
"manager": "US.3m.TR",
"perf": 0.0045,
"cumul": 1.2088 
},
{
 "date":  10895,
"manager": "US.3m.TR",
"perf": 0.00394,
"cumul": 1.2135 
},
{
 "date":  10925,
"manager": "US.3m.TR",
"perf":  0.004,
"cumul": 1.2184 
},
{
 "date":  10956,
"manager": "US.3m.TR",
"perf": 0.00448,
"cumul": 1.2239 
},
{
 "date":  10987,
"manager": "US.3m.TR",
"perf": 0.0043,
"cumul": 1.2291 
},
{
 "date":  11016,
"manager": "US.3m.TR",
"perf": 0.00438,
"cumul": 1.2345 
},
{
 "date":  11047,
"manager": "US.3m.TR",
"perf": 0.00521,
"cumul": 1.2409 
},
{
 "date":  11077,
"manager": "US.3m.TR",
"perf": 0.00466,
"cumul": 1.2467 
},
{
 "date":  11108,
"manager": "US.3m.TR",
"perf": 0.0061,
"cumul": 1.2543 
},
{
 "date":  11138,
"manager": "US.3m.TR",
"perf": 0.00431,
"cumul": 1.2597 
},
{
 "date":  11169,
"manager": "US.3m.TR",
"perf": 0.00454,
"cumul": 1.2655 
},
{
 "date":  11200,
"manager": "US.3m.TR",
"perf": 0.00518,
"cumul":  1.272 
},
{
 "date":  11230,
"manager": "US.3m.TR",
"perf": 0.00526,
"cumul": 1.2787 
},
{
 "date":  11261,
"manager": "US.3m.TR",
"perf": 0.0052,
"cumul": 1.2853 
},
{
 "date":  11291,
"manager": "US.3m.TR",
"perf": 0.00548,
"cumul": 1.2924 
},
{
 "date":  11322,
"manager": "US.3m.TR",
"perf": 0.00551,
"cumul": 1.2995 
},
{
 "date":  11353,
"manager": "US.3m.TR",
"perf": 0.00658,
"cumul": 1.3081 
},
{
 "date":  11381,
"manager": "US.3m.TR",
"perf": 0.00381,
"cumul":  1.313 
},
{
 "date":  11412,
"manager": "US.3m.TR",
"perf": 0.00459,
"cumul": 1.3191 
},
{
 "date":  11442,
"manager": "US.3m.TR",
"perf": 0.00439,
"cumul": 1.3249 
},
{
 "date":  11473,
"manager": "US.3m.TR",
"perf": 0.00388,
"cumul":   1.33 
},
{
 "date":  11503,
"manager": "US.3m.TR",
"perf": 0.00292,
"cumul": 1.3339 
},
{
 "date":  11534,
"manager": "US.3m.TR",
"perf": 0.00329,
"cumul": 1.3383 
},
{
 "date":  11565,
"manager": "US.3m.TR",
"perf": 0.00325,
"cumul": 1.3426 
},
{
 "date":  11595,
"manager": "US.3m.TR",
"perf": 0.00425,
"cumul": 1.3483 
},
{
 "date":  11626,
"manager": "US.3m.TR",
"perf": 0.00261,
"cumul": 1.3519 
},
{
 "date":  11656,
"manager": "US.3m.TR",
"perf": 0.00219,
"cumul": 1.3548 
},
{
 "date":  11687,
"manager": "US.3m.TR",
"perf": 0.00156,
"cumul": 1.3569 
},
{
 "date":  11718,
"manager": "US.3m.TR",
"perf": 0.00146,
"cumul": 1.3589 
},
{
 "date":  11746,
"manager": "US.3m.TR",
"perf": 0.00134,
"cumul": 1.3607 
},
{
 "date":  11777,
"manager": "US.3m.TR",
"perf": 0.0015,
"cumul": 1.3628 
},
{
 "date":  11807,
"manager": "US.3m.TR",
"perf": 0.00157,
"cumul": 1.3649 
},
{
 "date":  11838,
"manager": "US.3m.TR",
"perf": 0.00157,
"cumul": 1.3671 
},
{
 "date":  11868,
"manager": "US.3m.TR",
"perf": 0.00145,
"cumul":  1.369 
},
{
 "date":  11899,
"manager": "US.3m.TR",
"perf": 0.00153,
"cumul": 1.3711 
},
{
 "date":  11930,
"manager": "US.3m.TR",
"perf": 0.0014,
"cumul":  1.373 
},
{
 "date":  11960,
"manager": "US.3m.TR",
"perf": 0.0016,
"cumul": 1.3752 
},
{
 "date":  11991,
"manager": "US.3m.TR",
"perf": 0.00149,
"cumul": 1.3773 
},
{
 "date":  12021,
"manager": "US.3m.TR",
"perf": 0.0016,
"cumul": 1.3795 
},
{
 "date":  12052,
"manager": "US.3m.TR",
"perf": 0.00117,
"cumul": 1.3811 
},
{
 "date":  12083,
"manager": "US.3m.TR",
"perf": 0.00099,
"cumul": 1.3825 
},
{
 "date":  12111,
"manager": "US.3m.TR",
"perf": 0.00087,
"cumul": 1.3837 
},
{
 "date":  12142,
"manager": "US.3m.TR",
"perf": 0.00118,
"cumul": 1.3853 
},
{
 "date":  12172,
"manager": "US.3m.TR",
"perf": 0.00094,
"cumul": 1.3866 
},
{
 "date":  12203,
"manager": "US.3m.TR",
"perf":  0.001,
"cumul":  1.388 
},
{
 "date":  12233,
"manager": "US.3m.TR",
"perf": 0.0014,
"cumul": 1.3899 
},
{
 "date":  12264,
"manager": "US.3m.TR",
"perf": 0.00067,
"cumul": 1.3909 
},
{
 "date":  12295,
"manager": "US.3m.TR",
"perf": 0.00079,
"cumul":  1.392 
},
{
 "date":  12325,
"manager": "US.3m.TR",
"perf":  0.001,
"cumul": 1.3934 
},
{
 "date":  12356,
"manager": "US.3m.TR",
"perf": 0.00076,
"cumul": 1.3944 
},
{
 "date":  12386,
"manager": "US.3m.TR",
"perf": 0.00084,
"cumul": 1.3956 
},
{
 "date":  12417,
"manager": "US.3m.TR",
"perf": 0.00096,
"cumul": 1.3969 
},
{
 "date":  12448,
"manager": "US.3m.TR",
"perf": 0.00082,
"cumul": 1.3981 
},
{
 "date":  12477,
"manager": "US.3m.TR",
"perf": 0.00073,
"cumul": 1.3991 
},
{
 "date":  12508,
"manager": "US.3m.TR",
"perf": 0.00084,
"cumul": 1.4003 
},
{
 "date":  12538,
"manager": "US.3m.TR",
"perf": 0.00084,
"cumul": 1.4015 
},
{
 "date":  12569,
"manager": "US.3m.TR",
"perf": 0.00086,
"cumul": 1.4027 
},
{
 "date":  12599,
"manager": "US.3m.TR",
"perf": 0.00066,
"cumul": 1.4036 
},
{
 "date":  12630,
"manager": "US.3m.TR",
"perf": 0.00115,
"cumul": 1.4052 
},
{
 "date":  12661,
"manager": "US.3m.TR",
"perf": 0.00124,
"cumul": 1.4069 
},
{
 "date":  12691,
"manager": "US.3m.TR",
"perf": 0.00127,
"cumul": 1.4087 
},
{
 "date":  12722,
"manager": "US.3m.TR",
"perf": 0.0013,
"cumul": 1.4106 
},
{
 "date":  12752,
"manager": "US.3m.TR",
"perf": 0.00136,
"cumul": 1.4125 
},
{
 "date":  12783,
"manager": "US.3m.TR",
"perf": 0.00213,
"cumul": 1.4155 
},
{
 "date":  12814,
"manager": "US.3m.TR",
"perf": 0.00167,
"cumul": 1.4179 
},
{
 "date":  12842,
"manager": "US.3m.TR",
"perf": 0.00162,
"cumul": 1.4201 
},
{
 "date":  12873,
"manager": "US.3m.TR",
"perf": 0.00243,
"cumul": 1.4236 
},
{
 "date":  12903,
"manager": "US.3m.TR",
"perf": 0.00225,
"cumul": 1.4268 
},
{
 "date":  12934,
"manager": "US.3m.TR",
"perf": 0.00259,
"cumul": 1.4305 
},
{
 "date":  12964,
"manager": "US.3m.TR",
"perf": 0.0023,
"cumul": 1.4338 
},
{
 "date":  12995,
"manager": "US.3m.TR",
"perf": 0.00235,
"cumul": 1.4372 
},
{
 "date":  13026,
"manager": "US.3m.TR",
"perf": 0.0029,
"cumul": 1.4413 
},
{
 "date":  13056,
"manager": "US.3m.TR",
"perf": 0.00299,
"cumul": 1.4456 
},
{
 "date":  13087,
"manager": "US.3m.TR",
"perf": 0.00264,
"cumul": 1.4495 
},
{
 "date":  13117,
"manager": "US.3m.TR",
"perf": 0.00329,
"cumul": 1.4542 
},
{
 "date":  13148,
"manager": "US.3m.TR",
"perf": 0.00324,
"cumul": 1.4589 
},
{
 "date":  13179,
"manager": "US.3m.TR",
"perf": 0.00309,
"cumul": 1.4634 
},
{
 "date":  13207,
"manager": "US.3m.TR",
"perf": 0.00325,
"cumul": 1.4682 
},
{
 "date":  13238,
"manager": "US.3m.TR",
"perf": 0.00385,
"cumul": 1.4738 
},
{
 "date":  13268,
"manager": "US.3m.TR",
"perf": 0.00366,
"cumul": 1.4792 
},
{
 "date":  13299,
"manager": "US.3m.TR",
"perf": 0.00404,
"cumul": 1.4852 
},
{
 "date":  13329,
"manager": "US.3m.TR",
"perf": 0.00384,
"cumul": 1.4909 
},
{
 "date":  13360,
"manager": "US.3m.TR",
"perf": 0.00423,
"cumul": 1.4972 
},
{
 "date":  13391,
"manager": "US.3m.TR",
"perf": 0.00441,
"cumul": 1.5038 
},
{
 "date":  13421,
"manager": "US.3m.TR",
"perf": 0.00456,
"cumul": 1.5107 
},
{
 "date":  13452,
"manager": "US.3m.TR",
"perf": 0.00381,
"cumul": 1.5164 
},
{
 "date":  13482,
"manager": "US.3m.TR",
"perf": 0.0043,
"cumul":  1.523 
},
{
 "date":  13513,
"manager": "US.3m.TR",
"perf": 0.00441,
"cumul": 1.5297 
} 
]

)
</script>
