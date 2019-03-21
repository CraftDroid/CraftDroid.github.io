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
We have applied these fix templates on 20 apks selected from ReCBench, out of which 17 fixes are successful. 3 failed for various reasons. Viewing this commit for a diff view of the patches.

