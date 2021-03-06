# Model Gallery
Roughly 200 examples of how the model performed on the test set are visualized here, ordered by true county. Exploring the model predictions for a variety of input scenarios helps to give a sense of how the neural net is *thinking*. By looking at how the net treats colors, textures, and features over many test set examples, it is possible to start to see what it has learned and correlated with each county. Not all counties are presented. 

### Some highlights: 
 * The net gets all of the [Rio Blanco](#rio-blanco) test images right, and is very confident, guessing effectively 100% in each case. 
 * The net gets nearly all of the [Routt](#routt) test images correct, even though there is a significant amount of variety in the input landscapes. The one that it misses, it guesses neighboring Moffat. 
 * The net correctly guesses [Denver](#denver)'s test images as being from Denver in two of three cases. On the miss, it is still in the correct general area of Colorado. 
 * The net gets all of the [Saguache](#saguache) landscapes correct, though to be fair, these images all look like they are from the same google street view drive on the same cloudy day. A perfect example of the danger of the net learning the lighting more effectively than the landscape. To combat this, I'd want to utilize data from a variety of seasons and weather conditions, but this is beyond the ability of google street view imagery. 

### Some lowlights/other thoughts:
 * The net, overall, performs well on the [Weld](#weld) county examples, but some bizarre trends emerge. The 1th and 2th images seem to have the same features, but offset in direction (the E/W images in 1 are like the N/S images in 2), and this completely changes the prediction of the net. This seems to say that the net does not have a high level of abstraction with regards to features coming from each cardinal direction-- if it finds specific patterns between features among the cardinal directions in the training set, it will only assign a high similarity if the test image has the same features in the same orientation. 
 * The net goes 0/6 for [Teller](#teller) county. For one of these, the net ascertains that it is in the top 5, but for the rest, it is off, although a county with a high predicted probability is neighboring in 3 of the 6 examples. Then again, these images *are* pretty generic Colorado. 
 * 0/3 in [Summit](#summit) county. I think the net was mostly trained with snowy images from Summit, so when it sees mountainous but not very snowy landscapes (as is the case in these three random test set examples), it doesn't guess here. 
 * Hit or miss in [Mesa](#mesa) county. Sometimes right on, sometimes right nextdoor (guessing Garfield to the north), and sometimes halfway across the state. 


## List of Counties
 * [Adams](#adams)
 * [Arapahoe](#arapahoe)
 * [Baca](#baca)
 * [Bent](#bent)
 * [Boulder](#boulder)
 * [Chaffee](#chaffee)
 * [Clear Creek](#clear-creek)
 * [Crowley](#chaffee)
 * [Delta](#delta)
 * [Denver](#denver)
 * [Dolores](#dolores)
 * [Douglas](#douglas)
 * [Eagle](#eagle)
 * [El Paso](#el-paso)
 * [Elbert](#elbert)
 * [Garfield](#garfield)
 * [Grand](#grand)
 * [Gunnison](#gunnison)
 * [Huerfano](#huerfano)
 * [Jefferson](#jefferson)
 * [La Plata](#la-plata)
 * [Lake](#lake)
 * [Larimer](#larimer)
 * [Los Animas](#los-animas)
 * [Lincoln](#lincoln)
 * [Logan](#logan)
 * [Mesa](#mesa)
 * [Moffat](#moffat)
 * [Montezuma](#montezuma)
 * [Montrose](#montrose)
 * [Otero](#otero)
 * [Park](#park)
 * [Prowers](#prowers)
 * [Pueblo](#pueblo)
 * [Rio Blanco](#rio-blanco)
 * [Rio Grande](#rio-grande)
 * [Routt](#routt)
 * [Saguache](#saguache)
 * [Summit](#summit)
 * [Teller](#teller)
 * [Washington](#washington)
 * [Weld](#weld)

## Adams
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_525.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_531.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_544.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_551.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_583.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_613.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_618.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_641.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_653.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Adams_idx_694.png)
## Arapahoe
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_505.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_518.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_521.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_534.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_568.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_574.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_575.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_579.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_581.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_604.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Arapahoe_idx_607.png)
## Baca
![Image](/model_gallery/county_model_v1.3_newtruecolors_Baca_idx_539.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Baca_idx_606.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Baca_idx_646.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Baca_idx_663.png)
## Bent
![Image](/model_gallery/county_model_v1.3_newtruecolors_Bent_idx_527.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Bent_idx_609.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Bent_idx_647.png)
## Boulder
![Image](/model_gallery/county_model_v1.3_newtruecolors_Boulder_idx_509.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Boulder_idx_532.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Boulder_idx_603.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Boulder_idx_636.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Boulder_idx_683.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Boulder_idx_687.png)
## Chaffee
![Image](/model_gallery/county_model_v1.3_newtruecolors_Chaffee_idx_665.png)
## Clear Creek
![Image](/model_gallery/county_model_v1.3_newtruecolors_Clear Creek_idx_522.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Clear Creek_idx_593.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Clear Creek_idx_595.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Clear Creek_idx_610.png)
## Crowley
![Image](/model_gallery/county_model_v1.3_newtruecolors_Crowley_idx_672.png)
## Delta
![Image](/model_gallery/county_model_v1.3_newtruecolors_Delta_idx_552.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Delta_idx_664.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Delta_idx_675.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Delta_idx_689.png)
## Denver
![Image](/model_gallery/county_model_v1.3_newtruecolors_Denver_idx_622.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Denver_idx_624.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Denver_idx_628.png)
## Dolores
![Image](/model_gallery/county_model_v1.3_newtruecolors_Dolores_idx_657.png)
## Douglas
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_538.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_540.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_547.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_567.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_619.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_626.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Douglas_idx_627.png)
## Eagle
![Image](/model_gallery/county_model_v1.3_newtruecolors_Eagle_idx_557.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Eagle_idx_558.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Eagle_idx_560.png)
## El Paso
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_508.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_537.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_549.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_556.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_559.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_597.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_598.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_612.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_631.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_651.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_656.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_678.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_680.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_El Paso_idx_696.png)
## Elbert
![Image](/model_gallery/county_model_v1.3_newtruecolors_Elbert_idx_502.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Elbert_idx_504.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Elbert_idx_554.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Elbert_idx_589.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Elbert_idx_649.png)
## Garfield
![Image](/model_gallery/county_model_v1.3_newtruecolors_Garfield_idx_573.png)
## Grand
![Image](/model_gallery/county_model_v1.3_newtruecolors_Grand_idx_513.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Grand_idx_517.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Grand_idx_681.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Grand_idx_688.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Grand_idx_693.png)
## Gunnison
![Image](/model_gallery/county_model_v1.3_newtruecolors_Gunnison_idx_673.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Gunnison_idx_692.png)
## Huerfano
![Image](/model_gallery/county_model_v1.3_newtruecolors_Huerfano_idx_510.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Huerfano_idx_536.png)
## Jefferson
![Image](/model_gallery/county_model_v1.3_newtruecolors_Jefferson_idx_550.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Jefferson_idx_666.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Jefferson_idx_684.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Jefferson_idx_685.png)
## La Plata
![Image](/model_gallery/county_model_v1.3_newtruecolors_La Plata_idx_506.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_La Plata_idx_658.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_La Plata_idx_677.png)
## Lake
![Image](/model_gallery/county_model_v1.3_newtruecolors_Lake_idx_516.png)
## Larimer
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_501.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_503.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_511.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_515.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_530.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_564.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_587.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_638.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_644.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_686.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Larimer_idx_691.png)
## Los Animas
![Image](/model_gallery/county_model_v1.3_newtruecolors_Las Animas_idx_643.png)
## Lincoln
![Image](/model_gallery/county_model_v1.3_newtruecolors_Lincoln_idx_633.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Lincoln_idx_637.png)
## Logan
![Image](/model_gallery/county_model_v1.3_newtruecolors_Logan_idx_542.png)
## Mesa
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_553.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_562.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_566.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_571.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_572.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_588.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_590.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_592.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_640.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Mesa_idx_698.png)
## Moffat
![Image](/model_gallery/county_model_v1.3_newtruecolors_Moffat_idx_621.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Moffat_idx_630.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Moffat_idx_639.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Moffat_idx_654.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Moffat_idx_674.png)
## Montezuma
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montezuma_idx_580.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montezuma_idx_615.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montezuma_idx_629.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montezuma_idx_635.png)
## Montrose
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_533.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_608.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_617.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_625.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_632.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_655.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Montrose_idx_668.png)
## Otero
![Image](/model_gallery/county_model_v1.3_newtruecolors_Otero_idx_584.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Otero_idx_611.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Otero_idx_662.png)
## Park
![Image](/model_gallery/county_model_v1.3_newtruecolors_Park_idx_576.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Park_idx_585.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Park_idx_601.png)
## Prowers
![Image](/model_gallery/county_model_v1.3_newtruecolors_Prowers_idx_650.png)
## Pueblo
![Image](/model_gallery/county_model_v1.3_newtruecolors_Pueblo_idx_546.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Pueblo_idx_569.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Pueblo_idx_577.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Pueblo_idx_582.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Pueblo_idx_634.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Pueblo_idx_642.png)
## Rio Blanco
![Image](/model_gallery/county_model_v1.3_newtruecolors_Rio Blanco_idx_528.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Rio Blanco_idx_529.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Rio Blanco_idx_616.png)
## Rio Grande
![Image](/model_gallery/county_model_v1.3_newtruecolors_Rio Grande_idx_543.png)
## Routt
![Image](/model_gallery/county_model_v1.3_newtruecolors_Routt_idx_507.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Routt_idx_519.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Routt_idx_545.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Routt_idx_555.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Routt_idx_671.png)
## Saguache
![Image](/model_gallery/county_model_v1.3_newtruecolors_Saguache_idx_541.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Saguache_idx_599.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Saguache_idx_605.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Saguache_idx_661.png)
## Summit
![Image](/model_gallery/county_model_v1.3_newtruecolors_Summit_idx_548.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Summit_idx_565.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Summit_idx_596.png)
## Teller
![Image](/model_gallery/county_model_v1.3_newtruecolors_Teller_idx_500.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Teller_idx_514.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Teller_idx_520.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Teller_idx_523.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Teller_idx_570.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Teller_idx_623.png)
## Washington
![Image](/model_gallery/county_model_v1.3_newtruecolors_Washington_idx_524.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Washington_idx_594.png)
## Weld
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_600.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_602.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_526.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_535.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_561.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_563.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_578.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_586.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_591.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_614.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_620.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_645.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_648.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_652.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_660.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_667.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_669.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_670.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_676.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_679.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_682.png)
![Image](/model_gallery/county_model_v1.3_newtruecolors_Weld_idx_695.png)
