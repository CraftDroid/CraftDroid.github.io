## CraftDroid and ReCBench
### CraftDroid
CraftDroid is an approach for minging crash-inducing bug fixes in Android apps. As depicted in the Figuire below.
              ![CraftDroid](workflowCraftDroid.png)
### ReCBench
ReCBench is a collection of 200 Android crashed apps (where you must download from [AndroZoo](https://androzoo.uni.lu) with the sha256 provided for each apk) with crash reproducing script and crash message filtered out from LogCat.
The dataset is accessible [here](https://github.com/CraftDroid/ReCBench).

### Experimental Data
#### Fix Templates
We have mined 17 fix templates that are accessible [here](https://github.com/CraftDroid/ExpData/tree/master/Fix_Templates).
#### Evaluated Patches
We have applied these fix templates on 20 apks selected from ReCBench, out of which 17 fixes are successful. 3 failed for various reasons. Click on the app names for a diff view of the patches. (Quickly updating links 21-03-2019, kindly wait)

App Name |Bucket| Applied Template | Fix | Remark|
|-------|------|---------|------|------|
AutoHome | 8 |LifeCycle Verifier | yes |   |
PI | 8| LifeCycle Verifier | yes | |
JadwalKA |12| Thread Finisher | yes | |
Fruit Mahjong |12| Thread Finisher | yes | |
Flashlight | 1 | Provider Checker | yes | | 
areain! | 1 |Provider Checker | yes | |
 WordPress |18| Range Checker | no | crash with succeeding API |
[Android Optimizer](https://github.com/CraftDroid/ExpData/commit/8ee947a913fc1397c6756b7d4eac917fd49593c7) |18| Range Checker | yes | |
[Mine\_mine](https://github.com/CraftDroid/ExpData/commit/dbdb8db7c9a4cb67ba7dd33beb1b61fd58539fa2) |20| Emptiness Checker | yes | |
SetCPU |20| Emptiness Checker | no | String null throw NPE|
FingerWQ | 23|Canvas Preconcator | no | app method non existing |
[BTCfx](https://github.com/CraftDroid/ExpData/commit/ca263e4f33077074f2801ae3b97cff673695381d) |15| Package Settler | yes | |
 MapCam | 15|Package Settler | yes | |
 Baby Piano |2| Activity Resolver | yes | |
 GK in Gujarati |2| Activity Resolver | yes | |
 Reflection | 2|Activity Resolver | yes | |
 UK Lotto | 2|Activity Resolver | yes | |
 Agile Buddy | 2|Activity Resolver | yes | |
 [HiYou Park](https://github.com/CraftDroid/ExpData/commit/189292caa667d5938b40601fba355545cd6133f1) | 33|Try-catcher | yes | |
 Sohu Weibo | 33|Try-catcher | yes | |

