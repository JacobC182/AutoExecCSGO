# AutoExecCSGO
A Template CS:GO Autoexec.cfg Script

//LAUNCH OPTIONS (Because Steam deletes them all the time :/ )
//-tickrate 128 -refresh 165 +exec autoexec.cfg

//autoexec.cfg CS:GO setup/config file
clear

echo "//////////////////////////"
echo "Running autoexec Setup Script..."

//run autoexec shortcut
	
	alias "setup" "exec autoexec"

//sensitivity

	m_rawinput 1
	sensitivity 0.5
	zoom_sensitivity_ratio_mouse 0.818933027098955175

//sound/mic

	voice_positional 1
	volume 0.3
	voice_enable 1
	
	snd_menumusic_volume 0
	snd_roundstart_volume 0
	snd_roundend_volume 0
	snd_mapobjective_volume 0
	snd_tensecondwarning_volume 0.03
	snd_deathcamera_volume 0
	snd_mvp_volume 0
	
//excuse for lag
	
	cl_interp 0
	cl_interp_ratio 1
	cl_interpolate 1
	rate 128000
	cl_cmdrate 128
	cl_updaterate 128

//crosshair

	crosshair 1
	cl_crosshairstyle 4
	cl_crosshairsize 2
	cl_crosshairthickness 1
	cl_crosshairgap -2
	cl_crosshair_drawoutline 0
	cl_crosshaircolor 5
	cl_crosshairalpha 255
	cl_crosshairdot 0
	cl_crosshair_sniper_width 2

//viewmodel

	cl_viewmodel_shift_left_amt "1.5"
	cl_viewmodel_shift_right_amt "0.75"
	viewmodel_fov "68"
	viewmodel_offset_x "2.5"
	viewmodel_offset_y "2.0"
	viewmodel_offset_z "-1.400000"
	viewmodel_recoil "1"
	cl_bob_lower_amt "21"
	cl_bobamt_lat "0.33"
	cl_bobamt_vert "0.14"
	cl_bobcycle "0.98"

//jumpthrow bind

	alias "+jumpthrow" "+jump;-attack; +jumpbindsound"
	alias "-jumpthrow" "-jump"
	bind n "+jumpthrow "
	
//Crosshair size toggle bind

	alias "crosshairsizetoggle" "toggle cl_crosshairsize 2 1000; +crosshairsound"
	bind l crosshairsizetoggle
	
//Scroll jump toggle

	alias scroll "bind mwheelup +jump; bind mwheeldown +jump"
	alias noscroll "bind mwheelup invprev; bind mwheeldown invnext"
//HUD
	
	cl_hud_color 10
	cl_drawhud 1
	cl_use_opens_buy_menu 0
	cl_hud_radar_scale "1.1"
	cl_radar_scale "0.4"
	cl_autowepswitch 0
	cl_showfps 2
	cl_color 3
	cl_hud_healthammo_style 1
	cl_disablehtmlmotd 1
	gameinstructor_enable 0
	
//Keyboard

	//Movement
		
		bind w "+forward"
		bind s "+back"
		bind a "+moveleft"
		bind d "+moveright"
		
		bind "ctrl" "+duck"; +low"
		bind "shift" "+speed"
	
	//Control
		
		bind r "+reload"
		bind e "+use; +lever"
		bind g "drop; +switch"
		bind q "lastinv; +flip"
		bind b "buymenu; +buysound"
		bind c "+voicerecord"
		
		bind "1" "slot1;+switch"
        bind "2" "slot2;+switch"
        bind "3" "slot3;+switch"
        bind "4" "slot4;+lever"
        bind "5" "slot5"
        bind "f" "+lookatweapon;+swipe"
		
		bind "v" "noclip; +lever"
		

// Half-life 2 Sounds lol

	alias +lever "playvol buttons/button17 .15"
    //BOUND TO E (USE)^^^
 
    alias +switch "playvol buttons/button18 .4"
    //BOUND TO G (DROP)^^^
 
    alias +slow "playvol buttons/lever7 .1"
    //BOUND TO SHIFT (SLOW)^^^
 
    alias +low "playvol buttons/combine_button2 .15"
    //BOUND TO CTRL (CROUCH)^^^ 
 
    alias +flip "playvol buttons/combine_button1 .3"
    //BOUND TO Q (QUICKSWITCH)^^^
 
    alias +swipe "playvol buttons/button9 .2"
    //BOUND TO F (INSPECT)^^^
	
	alias +leftsound "playvol common/left .3"
	//BOUND to A (LEFT) ^^^
	
	alias +rightsound "playvol common/right .3"
	//BOUND to D (RIGHT) ^^^
	
	alias +jumpbindsound "playvol buttons/blip2 .15"
	//BOUND to N (JUMPTHROW) ^^^
	
	alias +buysound "playvol ui/menu_back .3"
	//BOUND TO B (BUYMENU) ^^^
	
	alias +crosshairsound "playvol buttons/button24 .15"
	//BOUND TO L (TOGGLE CROSSHAIR SIZE ) ^^^

echo "HL-2 Sounds ON :)"
	
//Console Shortcuts

	alias "inf" "sv_infinite_ammo 1"
	
	alias "rs" "mp_restartgame 1"
	
	alias "lim" "mp_limitteams 0"
	
	alias "autobal" "mp_autoteambalance 0"
	
	alias "dc" "disconnect"
	
	alias nobot "bot_kick"
	
	alias "rndtime" "mp_roundtime 60; mp_roundtime_defuse 60; mp_roundtime_hostage 60"
	
	alias "share" "mp_drop_knife_enable 1; mp_drop_grenade_enable 1"
	
	alias "bhop" "toggle sv_autobunnyhopping 0 1"
	
	alias "tracers" "toggle sv_showimpacts 0 1; toggle sv_grenade_trajectory 0 1; sv_grenade_trajectory_time 15"
	
	alias "chill" "sv_cheats 1; healthshot_health 100; give weapon_healthshot; inf; lim; autobal; nobot; rndtime; drop; sv_autobunnyhopping 1; tracers; mp_buy_anywhere 1, mp_buytime 3600; mp_maxmoney 60000; mp_startmoney 60000; ammo_grenade_limit_total 5; mp_warmup_end 1"
	
	alias "botz" "map aim_botz"
	alias "aim1" "map tr_reflex_remake_v4-d2_hr"
	
	alias "norecoil" "weapon_recoil_scale 0; weapon_accuracy_nospread 1"
	
	alias "m" "toggle voice_scale 0 1"
	
//StdOut - Printing
	
	echo "██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	echo "Config Loaded - Shortcuts:"
	echo "//SHORTCUTS"
	echo "setup 	- run autoexec script"
	echo "██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	echo "dc 		- disconnect"
	echo "m 		- toggle mute voicechat"
	echo "scroll/noscroll	- toggle scroll jumping
	echo "██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	echo "inf 		- infinite ammo"
	echo "rs 		- restartgame"
	echo "lim 	   	- limit teams off,"
	echo "autobal 	- toggle autobalance teams"
	echo "rndtime 	- max round time - 1hr"
	echo "drop 		- enable grenade/knife drops"
	echo "bhop		- toggle autobhopping"
	echo "tracers 	- toggles bullet/grenade tracers/trajectories"
	echo "chill		- loads practice/chill/testing session config"
	echo "norecoil 	- turns off recoil and spread"
	echo "nobot		- kick bots
	echo "██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	echo "botz 		- load aim_botz map"
	echo "aim1 		- load bot training aim map"
	echo "██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	echo "//BINDS"
	echo "key N		- Jumpthrow bind
	echo "key L		- Toggle large crosshair
	echo "██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	echo "███████╗██╗  ██╗██╗██████╗ ███████╗
	echo "██╔════╝██║  ██║██║██╔══██╗██╔════╝
	echo "███████╗███████║██║██████╔╝█████╗  
	echo "╚════██║██╔══██║██║██╔══██╗██╔══╝  
	echo "███████║██║  ██║██║██████╔╝███████╗
	echo "╚══════╝╚═╝  ╚═╝╚═╝╚═════╝ ╚══════╝
	echo "██╗      ██████╗  █████╗ ██████╗ ███████╗██████╗ 
	echo "██║     ██╔═══██╗██╔══██╗██╔══██╗██╔════╝██╔══██╗
	echo "██║     ██║   ██║███████║██║  ██║█████╗  ██║  ██║
	echo "██║     ██║   ██║██╔══██║██║  ██║██╔══╝  ██║  ██║
	echo "███████╗╚██████╔╝██║  ██║██████╔╝███████╗██████╔╝
	echo "╚══════╝ ╚═════╝ ╚═╝  ╚═╝╚═════╝ ╚══════╝╚═════╝ 
	echo "██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗██╗
	echo "╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝╚═╝
	
