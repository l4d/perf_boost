Installation
------------------
1. Download ProdigySim's recording helper plugin [here](https://github.com/ProdigySim/recording_helpers/releases/download/v0.6/recording_helpers-0.6-l4d.zip) and extract both the .dll and .vdf files into your addons folder.         
*Skip this step if you already use the plugin.*    

2. Download **one** of the VPK files of your choice (only use 1 VPK):  
   **[performance.vpk](https://github.com/l4d/perf_boost/raw/master/performance.vpk)** ˑ Full performance VPK.    
   **[performance_b.vpk](https://github.com/l4d/perf_boost/raw/master/performance_b.vpk)** ˑ Performance VPK with blood particles enabled.    
   **[performance_c.vpk](https://github.com/l4d/perf_boost/raw/master/performance_c.vpk)** ˑ For people experiencing crashing on modded servers.    
   **[performance_d.vpk](https://github.com/l4d/perf_boost/raw/master/performance_d.vpk)** ˑ Modded servers crash fix with blood enabled.


3. Move the VPK file to the addons folder.

*Note: Remove the -lv (low violence) launch command if being used.*  
*Note: Changing resolutions resets parts of the cfg and requires a restart.*  
*Note: It's recommended that you use the 'High Performance' power plan in Windows.*

Version Guide
------------------
**[performance.vpk](https://github.com/l4d/perf_boost/raw/master/performance.vpk)** ˑ Full performance VPK.    
**[performance_b.vpk](https://github.com/l4d/perf_boost/raw/master/performance_b.vpk)** ˑ Performance VPK with blood particles enabled.    
**[performance_c.vpk](https://github.com/l4d/perf_boost/raw/master/performance_c.vpk)** ˑ For people experiencing crashing on modded servers.    
**[performance_d.vpk](https://github.com/l4d/perf_boost/raw/master/performance_d.vpk)** ˑ Crash fix and blood enabled.





Benchmarking
------------------
**Don't expect the huge gains you see below with inferior hardware.**  
All results based on a three run sum average.    
All results are from load with the survivor view vomited and a large horde attacking on DT Map1.  
All results are from a recorded demo file for consistency.  

Test Setup: i5 2500k @ 4ghz / gtx 970 ssc+ / 8gb 1866mhz cl8 / w10 x64   
Video Settings: Everything disabled / Effect Detail Medium / Multicore Enabled / Memory High / 1080p / fps_max 999    

         

> **L4D Without FPS Boost**  
 302 frames 1.360 seconds **221.97 fps ( 4.50 ms/f )** 24.489 fps variability

         

> **L4D With FPS Boost**  
>  302 frames 0.702 seconds **429.97 fps ( 2.32 ms/f )** 44.956 fps variability
>  
> - 93% increase in frames per second
> - 48% decrease in latency to display a fresh frame
> - ( 1 second = 1000 ms ( 1000 ms / 429.97 fps = 2.32 ms/f ) ) e.g.:
>  - 60 fps = 16.6 ms/f
>  - 120 fps  = 8.3 ms/f

> [Sample profile](https://raw.githubusercontent.com/l4d/perf_boost/master/vprof_sample.log) of a full map play-through.

         

> **L4D With FPS Boost, Threadpool Reserve 1**  
  302 frames 0.680 seconds **444.30 fps ( 2.25 ms/f)** 44.045 fps variability
 
> Settings a threadpool reserve will cause the client to hang when exiting the game, so it's left out of the config. If you'd like to use this, you will need to have a dedicated exit key bind that sets the threadpool to 0 then exits the game.

Optional Settings
---------
If you want fading ragdolls instead of instantly disappearing ragdolls, put `g_ragdoll_fadespeed 1` in your autoexec.

If you want less blurry textures and clearer spray images, put `mat_picmip 1` in your autoexec.

You can refer to the [Hidden CVAR](http://steamcommunity.com/sharedfiles/filedetails/?id=564185677) guide on Steam for more optional settings you can add to your autoexec.

Crashing
---------
If you experience random crashing, put `exec fix` in your autoexec.

Related L4D Stuff
------------------
- [L4D Hidden Console Variables Guide](http://steamcommunity.com/sharedfiles/filedetails/?id=564185677)
- [L4D Translucent Viewmodels Repo](https://github.com/l4d/trans_vmodels) 
- [L4D Black Particle Fix Repo](https://github.com/l4d/particle_fix)
- [L4D HUD Project Repo](https://github.com/l4d/hud)
