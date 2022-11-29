-- Decompiled with the Synapse X Luau decompiler.

local l__KnitPath__1 = require(game.ReplicatedStorage.ReplicatedModules.PathShortcuts).KnitPath;
local v2 = require(l__KnitPath__1.TableUtil);
local v3 = require(l__KnitPath__1.Trove);
local l__Output__4 = game.ReplicatedStorage.Remotes.Output;
({})[1] = 7070248368;
local v5 = {
	SummonedRun = 7037969480, 
	SummonedWalk = 6707573199
};
local v6 = {
	anims = {
		DefaultAnims = {
			Action = {
				Dash = 6630347677, 
				ForwardDash = 10451361960, 
				BackwardDash = 10451359576, 
				LeftDash = 10451363828, 
				RightDash = 10451365211, 
				DeathAnimation = 7070248368, 
				KnockbackLoop = 9528670485, 
				KnockbackEnd = 9528673913, 
				Grab = 10906128504, 
				Throw = 10906131878, 
				ThrowVictim = 10906132668
			}, 
			Movement = {
				Run = 7037969480, 
				Walk = 6707573199, 
				TimeAccel = 6630347677, 
				Jump = 6869804977, 
				Fall = 6869825077, 
				Land = 7748987343, 
				Glide = 8725053000, 
				SummonedRun = 9253103011, 
				SummonedWalk = 9253105582, 
				LowHPRun = 6939421746, 
				LowHPWalk = 6939421746
			}, 
			Idle = {
				Idle = 6630333014, 
				LowHPIdle = 6826152951
			}
		}, 
		Casey = {
			Action = {
				Bonk = 5842787243, 
				Swing = 5842788141, 
				PoseTransition = 5842947612, 
				PoseIdle = 5842946044, 
				Dash = 5841978909
			}, 
			Idle = {
				SummonedIdle = 5842783938
			}
		}, 
		GER = {
			Action = {
				["LMB-1"] = 8479407906, 
				["LMB-2"] = 8479409142, 
				["LMB-3"] = 8479410619, 
				["LMB-4"] = 8479412145, 
				Barrage = 9582592923, 
				["Barrage Finisher"] = 10315501556, 
				["Heavy Attack"] = 10315506602, 
				["Return To Zero"] = 10315504361, 
				["Debris Projectile"] = 10315510337, 
				["Life Giver"] = 10315514494, 
				["Unreachable Truth"] = 10315516416, 
				["Pursuit Rush"] = 10315523095, 
				["Berserk Senses V2 Windup"] = 10620214430, 
				["Berserk Senses V2 User"] = 10620217492, 
				["Berserk Senses V2 Victim"] = 10620219985, 
				["Berserk Senses V2 Camera"] = 10620231495, 
				["Berserk Senses V2 Knockback"] = 10620235578, 
				WhaStartup = 10620237604, 
				WhaIdle = 10620238972
			}, 
			Idle = {
				Idle = 7193377883
			}
		}, 
		Clown = {
			Action = {
				["LMB-1"] = 5143367853, 
				["LMB-2"] = 5143376290, 
				["LMB-3"] = 5143367853, 
				["LMB-4"] = 5143376290, 
				Barrage = 10548807775, 
				TimeStop = 5146277255, 
				StrongPunch = 5965700661, 
				StandJump = 5889373753, 
				Block = 5922378153, 
				["Time Erase"] = 6789950709, 
				PilotUserIdle = 10035919728, 
				PilotUserTransition = 10035917372, 
				PilotForwardDash = 10128375083, 
				PilotBackwardDash = 10128373129, 
				PilotLeftDash = 10128376957, 
				PilotRightDash = 10128378333
			}, 
			Movement = {
				Walk = 10158780189, 
				SummonedWalk = 10158780189, 
				SummonedRun = 7037969480
			}, 
			Idle = {
				StandIdle = 5778922246, 
				Idle = 5778922246
			}
		}, 
		Anshen = {
			Action = {
				PoseTransition = 10583694475, 
				PoseIdle = 10583695744, 
				["LMB-1"] = 10584173915, 
				["LMB-2"] = 10584174823, 
				["LMB-3"] = 10584175663, 
				["LMB-4"] = 10584176570, 
				["Counter-Startup"] = 10558960348, 
				["Counter-Hit"] = 9217197796, 
				ConsecutiveSlashes = 10584122382
			}, 
			Movement = {
				SummonedRun = 8303099403, 
				SummonedWalk = 8303100740
			}, 
			Idle = {
				SummonedIdle = 8303096030
			}
		}, 
		Anshen_R = {
			Action = {
				PoseTransition = 10583694475, 
				PoseIdle = 10583695744, 
				["LMB-1"] = 10584173915, 
				["LMB-2"] = 10584174823, 
				["LMB-3"] = 10584175663, 
				["LMB-4"] = 10584176570, 
				["Counter-Startup"] = 10558960348, 
				["Counter-Hit"] = 9217197796, 
				ConsecutiveSlashes = 10584122382, 
				Summon = 8269567032, 
				AcceleratedSwing = 8099605049, 
				SwiftWings = 8269661162, 
				Swing = 8118489878, 
				Throw = 8118487070, 
				EnergyCharge = 8269577491, 
				LanceRetrieval = 8118482919, 
				LanceAttack = 8118477962, 
				CataclysmSmashWind = 8099627588, 
				CataclysmSmashAssault = 8099633176, 
				JusticeWindup = 8118460630, 
				Execution = 8152935668
			}, 
			Movement = {
				SummonedRun = 8303099403, 
				SummonedWalk = 8303100740
			}, 
			Idle = {
				SummonedIdle = 8303096030
			}
		}, 
		A_Sans = {
			Action = {
				["Bone Field"] = 7272561672
			}, 
			Movement = {
				Run = 7272215238, 
				Walk = 7272215843
			}, 
			Idle = {
				Idle = 7272213387
			}
		}, 
		Ruined = {
			Action = {
				["LMB-1"] = 9914915906, 
				["LMB-2"] = 9914916923, 
				["LMB-3"] = 9914918056, 
				Equip = 9914912617, 
				Thrust = 9944762298
			}, 
			Movement = {
				SummonedWalk = 9914920142, 
				SummonedRun = 9924817196, 
				Run = 7272215238, 
				Walk = 7339784680
			}, 
			Idle = {
				SummonedIdle = 9944492483, 
				Idle = 9944508260
			}
		}, 
		Kars = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				["Ricochet Storm"] = 10858574405, 
				["Bug Crusher"] = 10900235680, 
				["Guttural Implant"] = 10900239042, 
				["Cruel Ambitions"] = 10253568916, 
				["Blade Technique"] = 10900229544, 
				["Heart and Saber"] = 10548745883, 
				["Flash of Light"] = 10023491451, 
				["Assassin's Blade"] = 10277629893, 
				PoseStart = 10373588196, 
				PoseLoop = 10373590219
			}, 
			Movement = {
				Walk = 10023136479, 
				Run = 10023208024
			}, 
			Idle = {
				Idle = 10023130672
			}
		}, 
		Vampire = {
			Action = {}, 
			Movement = {
				Walk = 10653285141, 
				Run = 10653283636
			}, 
			Idle = {
				Idle = 10653317287
			}
		}, 
		["Jonathan Hamon"] = {
			Action = {
				["LMB-1"] = 10452669137, 
				["LMB-2"] = 10452673192, 
				["LMB-3"] = 10452679412, 
				["LMB-4"] = 10452683994, 
				["Pluck LMB-1"] = 10487136143, 
				["Pluck LMB-2"] = 10487140752, 
				["Pluck LMB-3"] = 10487145423, 
				["Pluck LMB-4"] = 10487151401, 
				["Hamon Charge Startup"] = 10441557592, 
				["Hamon Charge Loop"] = 10441559558, 
				["Overdrive Barrage Startup"] = 10465745114, 
				["Overdrive Barrage Looped"] = 10465754588, 
				["Overdrive Barrage Finisher"] = 10465750030, 
				["Steel Blade"] = 10491716782, 
				["Eternal Heart Startup"] = 10481651657, 
				["Eternal Heart Finisher"] = 10481659008, 
				["Thorn Splicer"] = 10482107850, 
				["Zoom Punch"] = 10466205576, 
				["Luck Startup"] = 10502648976, 
				["Luck Hit"] = 10502652638, 
				["Luck Victim"] = 10502645638, 
				["Righteous Fury Startup"] = 10523113554, 
				["Righteous Fury Hit"] = 10523134118, 
				["Righteous Fury Victim"] = 10523136400, 
				Pluck = 10493395328, 
				["Luck & Pluck Equip"] = 10481736577, 
				["Luck & Pluck Unequip"] = 10481757171, 
				["Sunlight Yellow Overdrive"] = 10580573654, 
				["Metal Silver Overdrive"] = 10494294104, 
				["Sendo Ripple Overdrive"] = 10539686054
			}, 
			Movement = {
				Walk = 10344439263, 
				Run = 10344441371, 
				["Pluck Walk"] = 10481741482, 
				["Pluck Run"] = 10481745496
			}, 
			Idle = {
				Idle = 10344437299, 
				["Pluck Idle"] = 10481749940
			}
		}, 
		["Jonathan Hamon NEW"] = {
			Action = {
				["LMB-1"] = 10452669137, 
				["LMB-2"] = 10452673192, 
				["LMB-3"] = 10452679412, 
				["LMB-4"] = 10452683994, 
				["Pluck LMB-1"] = 10487136143, 
				["Pluck LMB-2"] = 10487140752, 
				["Pluck LMB-3"] = 10487145423, 
				["Pluck LMB-4"] = 10487151401, 
				["Hamon Charge Startup"] = 10441557592, 
				["Hamon Charge Loop"] = 10441559558, 
				["Overdrive Barrage Startup"] = 10465745114, 
				["Overdrive Barrage Looped"] = 10465754588, 
				["Overdrive Barrage Finisher"] = 10465750030, 
				["Steel Blade"] = 10491716782, 
				["Eternal Heart Startup"] = 10481651657, 
				["Eternal Heart Finisher"] = 10481659008, 
				["Thorn Splicer"] = 10482107850, 
				["Zoom Punch"] = 10466205576, 
				["Luck Startup"] = 10502648976, 
				["Luck Hit"] = 10502652638, 
				["Luck Victim"] = 10502645638, 
				["Righteous Fury Startup"] = 10523113554, 
				["Righteous Fury Hit"] = 10523134118, 
				["Righteous Fury Victim"] = 10523136400, 
				Pluck = 10493395328, 
				["Luck & Pluck Equip"] = 10481736577, 
				["Luck & Pluck Unequip"] = 10481757171, 
				["Sunlight Yellow Overdrive"] = 10580573654, 
				["Metal Silver Overdrive"] = 10494294104, 
				["Sendo Ripple Overdrive"] = 10539686054, 
				Grab = 11159544716, 
				Throw = 11159545307, 
				ThrowVictim = 11159546054, 
				PoseIdle = 11159566929, 
				PoseTransition = 11159565402, 
				PluckPoseIdle = 11159594979, 
				PluckPoseTransition = 11159564007
			}, 
			Movement = {
				Walk = 10344439263, 
				Run = 10344441371, 
				["Pluck Walk"] = 10481741482, 
				["Pluck Run"] = 10481745496
			}, 
			Idle = {
				Idle = 10344437299, 
				["Pluck Idle"] = 10481749940
			}
		}, 
		Fightsabre = {
			Action = {
				Shoot = 5862021910, 
				Reload = 5862022700, 
				Kick = 5838698998, 
				PoseTransition = 5862209023, 
				PoseIdle = 5862227840, 
				Dash = 5841978909
			}, 
			Movement = {
				Jump = 5838597419
			}, 
			Idle = {
				Idle = 5862045131
			}
		}, 
		Gun = {
			Action = {
				Shoot = 5838363810, 
				Reload = 5838362834, 
				Kick = 5838698998, 
				PoseIdle = 5841873122, 
				PoseTransition = 5841947922, 
				Dash = 5841978909, 
				Whip = 5838608797
			}, 
			Movement = {
				Jump = 5838597419
			}, 
			Idle = {
				Idle = 5838374728
			}
		}, 
		Hornet = {
			Action = {
				Hegale = 6079529359, 
				Garama = 6079583891, 
				PoseTransition = 6079465430, 
				PoseIdle = 6079518530, 
				Edino = 6079526759, 
				AirDash = 6079473609, 
				["Dash Strike"] = 6079477125, 
				m1 = 6124409935
			}
		}, 
		EP_R = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				["StandOff-LMB-1"] = 11127865908, 
				["StandOff-LMB-2"] = 11127868260, 
				["StandOff-LMB-3"] = 11127869614, 
				["StandOff-LMB-4"] = 11127870798, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				Grab = 11159544716, 
				Throw = 11159545307, 
				ThrowVictim = 11159546054, 
				["Quote-1"] = 10976760361, 
				["Quote-2"] = 10976761195, 
				["Quote-3"] = 10976763020
			}, 
			Movement = {
				Walk = 10856503017, 
				Run = 10856500879, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				Idle = 10842851957
			}
		}, 
		["Slayer Armor II"] = {
			Action = {
				["LMB-1"] = 9489091712, 
				["LMB-2"] = 9489093677, 
				["LMB-3"] = 9489095046, 
				Equip = 9488041296
			}, 
			Movement = {
				SummonedWalk = 9488046140, 
				SummonedRun = 9488047574, 
				Walk = 8577083049, 
				Run = 8577096811
			}, 
			Idle = {
				SummonedIdle = 9488042741, 
				Idle = 6943911515
			}
		}, 
		["D4C: Love Train"] = {
			Action = {
				["LMB-1"] = 10290554639, 
				["LMB-2"] = 10290555363, 
				["LMB-3"] = 10290556057, 
				Summon = 8604415872, 
				["StandOff-LMB-1"] = 10307709714, 
				["StandOff-LMB-2"] = 10307711291, 
				["StandOff-LMB-3"] = 10307712737, 
				["StandOff-LMB-4"] = 10307738458, 
				LoveTrainStartup = 8675840017, 
				["Dimension Hide"] = 7851087001, 
				["Dimension Hide Exit"] = 7856121850, 
				["Dimension Beatdown User"] = 8488442914, 
				["Dimension Beatdown Victim"] = 8500522374, 
				["Dash Camera"] = 8695287751, 
				["Dash User"] = 8695862218, 
				["Dash Clone"] = 8695867476, 
				["Dash Victim"] = 8715135121, 
				["Dash Victim Clone"] = 8695872112, 
				["Severing Chokeslam Start"] = 8614164038, 
				["Severing Chokeslam"] = 8614827594, 
				["Severing Victim"] = 8614166899, 
				Chokeslammed = 8614169552, 
				PoseIdle = 8574228830, 
				PoseTransition = 8574225633, 
				["First Napkin"] = 10137381164, 
				["First Napkin Victim"] = 10137388962, 
				GunWindup = 10002442542, 
				FanfireDisposal = 10002444730, 
				PrecisionDisposal = 10002447207, 
				GutGougeWindup = 10002449906, 
				GutGouge = 10002452257, 
				GutGougeVictim = 10002454324, 
				BodyCarving = 10036276073, 
				SpillingOfBloodWindup = 10002462639, 
				SpillingOfBlood = 10002459558, 
				SpillingOfBloodVictim = 10002464833, 
				PilotUserIdle = 10035919728, 
				PilotUserTransition = 10035917372, 
				["State Funeral"] = 10086880269, 
				["State Funeral User"] = 10382989072, 
				["State Funeral Victim"] = 10382991168, 
				ChopStrike = 10138512331, 
				ChopStrikeStandOff = 10139619761, 
				PincerAttack = 10289504741, 
				IncisionAttempt = 10139358481, 
				Incision = 10139361358, 
				IncisionVictim = 10139364675, 
				HandOfFortuneUser = 10343445032, 
				HandOfFortuneStand = 10513677517, 
				HeadBomb = 10361194439, 
				PresidentialLeverage = 10466366249
			}, 
			Movement = {
				Walk = 8577083049, 
				Run = 8577096811, 
				SummonedWalk = 8577083049, 
				SummonedRun = 8577096811, 
				LoveTrainWalk = 7370960151, 
				LoveTrainRun = 7370961968
			}, 
			Idle = {
				StandIdle = 10286553949, 
				Idle = 10284132160, 
				LoveTrainIdle = 10284136033
			}
		}, 
		["Silver Chariot"] = {
			Action = {
				["LMB-1"] = 9754322259, 
				["LMB-2"] = 9754324260, 
				["LMB-3"] = 9754326370, 
				["LMB-4"] = 9754328810, 
				SummonAnim = 9571449255, 
				PoseIdle = 10395020276, 
				PoseTransition = 10395012228, 
				["Armor Off"] = 9754332079, 
				["Armor Off Idle"] = 10118566913, 
				["Rapier Thrusts"] = 10159962142, 
				["Rapier Thrusts Finisher"] = 10159965589, 
				["Skull Piercing Thrust Startup"] = 10216765477, 
				["Skull Piercing Thrust Stance"] = 9617463614, 
				["Skull Piercing Thrust Success"] = 9617465658, 
				["Instant Slice Hold"] = 9617467779, 
				["Instant Slice"] = 9617469445, 
				["Ricochet Shot"] = 9617472189, 
				["You're Lying"] = 9617474580, 
				["Eye Of The Storm Start"] = 10280037313, 
				["Eye Of The Storm Loop"] = 10280049266, 
				["Eye Of The Storm End"] = 10280056707, 
				["Piercing Finisher Attempt"] = 10593374578, 
				["Piercing Finisher Attack"] = 10593389885, 
				["Piercing Finisher Victim"] = 10593426309
			}, 
			Movement = v5, 
			Idle = {
				Idle = 9670537715, 
				StandIdle = 9670540318
			}
		}, 
		SC_R = {
			Action = {
				BarrageStartup = 10838298509, 
				Barrage = 10159962142, 
				BarrageFinisher = 10159965589, 
				BarrageClashEnd = 10839831781, 
				["LMB-1"] = 9754322259, 
				["LMB-2"] = 9754324260, 
				["LMB-3"] = 9754326370, 
				["LMB-4"] = 9754328810, 
				["StandOff-LMB-1"] = 11127865908, 
				["StandOff-LMB-2"] = 11127868260, 
				["StandOff-LMB-3"] = 11127869614, 
				["StandOff-LMB-4"] = 11127870798, 
				SummonAnim = 9571449255, 
				PoseIdle = 10395020276, 
				PoseTransition = 10395012228, 
				["Armor Off"] = 9754332079, 
				["Armor Off Idle"] = 10118566913, 
				["Skull Piercing Thrust Startup"] = 10216765477, 
				["Skull Piercing Thrust Stance"] = 9617463614, 
				["Skull Piercing Thrust Success"] = 9617465658, 
				["Instant Slice Hold"] = 9617467779, 
				["Instant Slice"] = 9617469445, 
				["Ricochet Shot"] = 9617472189, 
				["You're Lying"] = 9617474580, 
				["Eye Of The Storm Start"] = 10280037313, 
				["Eye Of The Storm Loop"] = 10959747857, 
				["Eye Of The Storm End"] = 10280056707, 
				TempPierceFinishStart = 10938760715, 
				TempPierceFinishLoop = 10938762256, 
				["Piercing Finisher Attempt"] = 10593374578, 
				["Piercing Finisher Attack"] = 10593389885, 
				["Piercing Finisher Victim"] = 10593426309, 
				["Triple Strike"] = 10967692379, 
				Clobber = 11163414930, 
				["Immobilizing Slices"] = 11163653420, 
				["Immobilizing Slices Succeeded"] = 11163658200, 
				["Immobilizing Slices Failed"] = 11163659709
			}, 
			Movement = {
				SummonedWalk = 6707573199, 
				SummonedRun = 7037969480, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 9670540318, 
				Idle = 9670537715
			}
		}, 
		["Crazy Diamond"] = {
			Action = {
				["One Two Combination"] = 9537064690, 
				["Pressure Cutter Use"] = 9546195951, 
				["Pressure Cutter Hit"] = 9546198152, 
				["Pressure Cutter Victim"] = 9546199214, 
				["Deadeye Shot"] = 9553449027, 
				["Diamond Crusher"] = 9582592923, 
				["Diamond Crusher Finisher"] = 9583147145, 
				["LMB-1"] = 9590350054, 
				["LMB-2"] = 9590352534, 
				["LMB-3"] = 9590355134, 
				["LMB-4"] = 9590357465, 
				["Lightning Jabs"] = 9808785066, 
				["Lightning Jabs Hit"] = 9808794686, 
				["Lightning Jabs Victim"] = 9808787463, 
				["Restoration Uppercut"] = 9740451895, 
				["Rising Star"] = 9872779855, 
				["Rising Star Victim"] = 9872781699, 
				["Line Breaker"] = 9592195864, 
				["Rock Wall Startup"] = 10014923485, 
				["Rock Wall Loop"] = 10014921292, 
				["Rock Wall End"] = 10014920050, 
				["Rock Wall Punch"] = 10384335661, 
				PoseIdle = 9904211228, 
				PoseTransition = 9904210034, 
				["Instigation Startup"] = 10429413163, 
				["Instigation Loop"] = 10429417151, 
				["Instigation Activation"] = 10429406778, 
				Block = 10053550381
			}, 
			Movement = {
				Walk = 9552978705, 
				Run = 9552977036, 
				SummonedWalk = 9552978705, 
				SummonedRun = 9552977036
			}, 
			Idle = {
				StandIdle = 9536615499, 
				Idle = 9536617649
			}
		}, 
		["Sakuya Izayoi"] = {
			Action = {
				PoseTransition = 7834580007, 
				PoseIdle = 7834581175, 
				["LMB-1"] = 8634036082, 
				["LMB-2"] = 8634037567, 
				["LMB-3"] = 8634039244
			}, 
			Idle = {
				Idle = 7082645315
			}
		}, 
		Killua = {
			Action = {
				["LMB-1"] = 7283574427, 
				["LMB-2"] = 7283575295, 
				["LMB-3"] = 7283576424, 
				["LMB-4"] = 7283577409, 
				NoMercyKick = 7284000061, 
				NoMercyLightningPalm = 7284003850, 
				AirLightning = 7284004774, 
				GroundLightning = 7284006262, 
				Snake = 7293096473, 
				InstantDeath = 7293594684, 
				GrabHeart = 7293596879, 
				OnslaughtWindup = 7406016749, 
				OnslaughtDash = 7406045618, 
				OnslaughtBD = 7406314237, 
				OnslaughtVictim = 7406302666, 
				Godspeed = 7415474339, 
				TeleportLightning = 7415921371, 
				PoseIdle = 8055488849, 
				PoseTransition = 8055486767
			}, 
			Movement = {
				Run = 7294685851, 
				Walk = 7294686634
			}, 
			Idle = {
				Idle = 7294684954
			}
		}, 
		["Planet Shaper"] = {
			Action = {
				["Chicxulub Asteroid"] = 8243744661, 
				["LMB-1"] = 8833858741, 
				["LMB-2"] = 8833863225, 
				["LMB-3"] = 8833858741, 
				["LMB-4"] = 8688528286, 
				Earthquake = 8688518639, 
				["Portal Pass"] = 8688528286, 
				Roar = 8689723794, 
				Grab = 8697691350, 
				PoseTransition = 8702974469, 
				PoseIdle = 8702976463, 
				SelfHeal = 8027965306, 
				TeamworkStart = 8765125585, 
				TeamworkUser = 8765233284, 
				TeamworkVictim = 8765130959, 
				Starstruck = 8769459761, 
				GateWarp = 8829306780
			}, 
			Idle = {
				StandIdle = 8273533330
			}
		}, 
		["PLANET // SHAPER"] = {
			Action = {
				["Chicxulub Asteroid"] = 8243744661, 
				["LMB-1"] = 8833858741, 
				["LMB-2"] = 8833863225, 
				["LMB-3"] = 8833858741, 
				["LMB-4"] = 8688528286, 
				Earthquake = 8688518639, 
				["Portal Pass"] = 8688528286, 
				Roar = 8689723794, 
				Grab = 8697691350, 
				PoseTransition = 8702974469, 
				PoseIdle = 8702976463, 
				SelfHeal = 8027965306, 
				TeamworkStart = 8765125585, 
				TeamworkUser = 8765233284, 
				TeamworkVictim = 8765130959, 
				Starstruck = 8769459761, 
				GateWarp = 8829306780
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 8273533330
			}
		}, 
		["P//S_R"] = {
			Action = {
				Summon = 11253115200, 
				Desummon = 11253119442, 
				VisceralAttack = 11255212632, 
				StarStrikeStartup = 11370425003, 
				StarStrikeLoop = 11370429463, 
				StarStrikeFinisher = 11370430676, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				BreakneckAssaultStart1 = 11275639615, 
				BreakneckAssaultStart2 = 11275642071, 
				BreakneckAssaultStart3 = 11275643669, 
				BreakneckAssaultStart4 = 11275645219, 
				BreakneckAssaultLoop1 = 11275648364, 
				BreakneckAssaultLoop2 = 11275650431, 
				BreakneckAssaultLoop3 = 11275652176, 
				BreakneckAssaultLoop4 = 11275652176, 
				BreakneckAssaultFinisher = 11275655470
			}, 
			Movement = {
				Walk = 11253113453, 
				Run = 11253111199, 
				SummonedWalk = 11197130211, 
				SummonedRun = 11197128590, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 11197124815, 
				Idle = 11253108111
			}
		}, 
		NS_R = {
			Action = {
				Summon = 11253115200, 
				Desummon = 11253119442, 
				VisceralAttack = 11255212632, 
				StarStrikeStartup = 11370425003, 
				StarStrikeLoop = 11370429463, 
				StarStrikeFinisher = 11370430676, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				BreakneckAssaultStart1 = 11275639615, 
				BreakneckAssaultStart2 = 11275642071, 
				BreakneckAssaultStart3 = 11275643669, 
				BreakneckAssaultStart4 = 11275645219, 
				BreakneckAssaultLoop1 = 11275648364, 
				BreakneckAssaultLoop2 = 11275650431, 
				BreakneckAssaultLoop3 = 11275652176, 
				BreakneckAssaultLoop4 = 11275652176, 
				BreakneckAssaultFinisher = 11275655470
			}, 
			Movement = {
				Walk = 11253113453, 
				Run = 11253111199, 
				SummonedWalk = 11197130211, 
				SummonedRun = 11197128590, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 11197124815, 
				Idle = 11253108111
			}
		}, 
		Galizur = {
			Action = {
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6761488706, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				Barrage = 6331004626, 
				HeavyPunch = 6944002089, 
				NeturalizationHeal = 6943327916, 
				["Reality Overwrite"] = 6954932822, 
				Timestop = 6943779788, 
				SelfHealUser = 6880380737, 
				ThunderGod = 6946096569, 
				Strike = 6950249628, 
				SweepKick = 6947703992, 
				KnifeThrow = 6947706039
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 7114359566
			}
		}, 
		Gaster = {
			Action = {
				Summon = 7125583123, 
				Core = 7125643137, 
				OLDCore = 5630216399, 
				DeSummon = 7125689200, 
				SelfHeal = 5629226076, 
				AllyHeal = 5629228404, 
				Slash = 5641408651, 
				Bullets = 5630120742, 
				Bombs = 5630323630, 
				Block = 7126320310, 
				Laser = 5641461493, 
				Saw = 5630087705, 
				Pully = 5629647334
			}, 
			Movement = {
				Walk = 5627215440
			}, 
			Idle = {
				Idle = 7125645251
			}
		}, 
		xChara = {
			Action = {
				["LMB-1"] = 7074784464, 
				["LMB-2"] = 7074785215, 
				["LMB-3"] = 7074785861, 
				Stab = 7074768593, 
				HeavyHit = 5888090779, 
				FunnyStab = 5838697879, 
				Uppercut = 5838699307, 
				OLDM1 = 5888090413, 
				OLDM2 = 5888090566, 
				GroundSlam = 7114553506, 
				Heal = 5854734790
			}, 
			Movement = {
				Run = 7074565976, 
				Walk = 7074566537
			}, 
			Idle = {
				Idle = 7074564343
			}
		}, 
		TWOH_R = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				["StandOff-LMB-1"] = 11127865908, 
				["StandOff-LMB-2"] = 11127868260, 
				["StandOff-LMB-3"] = 11127869614, 
				["StandOff-LMB-4"] = 11127870798, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				Grab = 10906128504, 
				Throw = 10906131878, 
				ThrowVictim = 10906132668, 
				["Heavy Punch"] = 11386536360, 
				["Round Kick"] = 10953924145, 
				["Behind and Above Startup"] = 11386251961, 
				["Behind and Above Loop"] = 11386253322, 
				["Behind and Above End"] = 11386254583, 
				Mangle = 10962400136, 
				["Rampage Force Startup"] = 11371960721, 
				["Rampage Force Success"] = 11371962866, 
				["Rampage Force Victim"] = 11371961601, 
				["Overwrite Infusion"] = 10983521106, 
				["Cataclysmic Throw"] = 11091663194, 
				Fissure = 11109820411, 
				["Immortal Strikes Startup"] = 11308201056, 
				["Immortal Strikes Success"] = 11308205429, 
				["Immortal Strikes Victim"] = 11308204753, 
				["Immortal Strikes Camera"] = 11372387197, 
				Timestop = 11274629341, 
				["Divine Thunder"] = 11274628314
			}, 
			Movement = {
				SummonedWalk = 10953884475, 
				SummonedRun = 10953882774, 
				Walk = 10953884475, 
				Run = 10953882774
			}, 
			Idle = {
				StandIdle = 10953881155, 
				Idle = 10953881155
			}
		}, 
		["The World: Over Heaven"] = {
			Action = {
				["LMB-1"] = 6942193924, 
				["LMB-2"] = 6942194844, 
				["LMB-3"] = 6942195599, 
				["LMB-4"] = 6942196256, 
				Barrage = 6331004626, 
				HeavyPunch = 6944002089, 
				NeturalizationHeal = 6943327916, 
				["Reality Overwrite"] = 6954932822, 
				Timestop = 6943779788, 
				SelfHealUser = 6880380737, 
				ThunderGod = 6946096569, 
				Strike = 6950249628, 
				SweepKick = 6947703992, 
				KnifeThrow = 6947706039, 
				PoseTransition = 8060217789, 
				PoseIdle = 8060216135
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6943969490, 
				Idle = 6943911515
			}
		}, 
		["Dragon Sage"] = {
			Action = {
				LElbow = 7086070490, 
				ThunderingLeap = 7086960243, 
				["LMB-1"] = 7087806959, 
				["LMB-2"] = 7087808284, 
				["LMB-3"] = 7087811086, 
				["LMB-4"] = 7087813864, 
				["LMB-5"] = 7087816245, 
				ElectricSmite = 7090411176, 
				GrabAttempt = 7092246633
			}
		}, 
		Ardoth = {
			Action = {
				LElbow = 7088221452, 
				ThunderingLeap = 7086960243, 
				["LMB-1"] = 7087806959, 
				["LMB-2"] = 7087808284, 
				["LMB-3"] = 7087811086, 
				["LMB-4"] = 7087813864, 
				["LMB-5"] = 7087816245
			}
		}, 
		D4C = {
			Action = {
				Gunshots = 6955684230, 
				Gunshot = 7081331191, 
				ReloadGun = 8513845878, 
				["LMB-1"] = 6942193924, 
				["LMB-2"] = 6942194844, 
				["LMB-3"] = 6942195599, 
				["LMB-4"] = 6942196256, 
				["StandOff-LMB-1"] = 6955620587, 
				["StandOff-LMB-2"] = 6955621861, 
				["StandOff-LMB-3"] = 8513845878, 
				["StandOff-LMB-4"] = 6955621861, 
				Barrage = 7041796217, 
				HeavyPunch = 7189349499, 
				TwoArmPunch = 7041819690, 
				Uppercut = 7080376767, 
				D4CSlam = 7080880379, 
				["Clone Bomb"] = 7081047669, 
				["Dimension Hop"] = 7091385791, 
				Run = 7037969480, 
				["Counter Startup"] = 7071462816, 
				["Jumper-1"] = 7071483574, 
				["Jumper-2"] = 7071482261, 
				Jumped = 7071485507, 
				PoseTransition = 10405284330, 
				PoseIdle = 10405289231
			}, 
			Movement = {
				Walk = 6877996750, 
				Run = 7037969480, 
				SummonedWalk = 6877996750, 
				SummonedRun = 7037969480
			}, 
			Idle = {
				StandIdle = 6954981919, 
				Idle = 6954960940
			}
		}, 
		Tusk = {
			Action = {
				Barrage = 7056069797, 
				["Strong Punch"] = 7364363789, 
				["Heavy Punch"] = 7209760261, 
				Scratch = 7024678264, 
				Glide = 7024676952, 
				NailShot = 7032002952, 
				Tea = 7058431247, 
				ChargedNailShot = 7032000229, 
				Wormhole = 6017451715, 
				StandUp = 7038048657, 
				BallEquip = 7039224922, 
				BallCharge = 7039210945, 
				BallRelease = 7039212218, 
				Block = 7052155676, 
				Sit = 5718959564, 
				TuskEnter = 7065554384, 
				TuskExit = 7065619313, 
				Slam = 7070621142, 
				Determination = 7071178699, 
				ShakingCamera = 10169802618, 
				Camera = 10169800701, 
				BeatdownVictim = 10153048045, 
				BeatdownTusk = 10153226033
			}, 
			Movement = {
				Run = 7037969480, 
				Walk = 6877996750
			}, 
			Idle = {
				Idle = 7473273038, 
				ACT1Idle = 5995500285, 
				ACT2Idle = 10382725748, 
				ACT3Idle = 10382743443, 
				ACT4Idle = 10382756362
			}
		}, 
		Sol = {
			Action = {
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				Barrage = 6925550526, 
				SolStarCombo = 6937462921, 
				BlackHole = 6925551881, 
				IntangiblePunch = 6925552789, 
				Forcefield = 6925553631, 
				["Pose Transition Stand"] = 7772889380, 
				["Pose Transition root"] = 7772891068, 
				["Pose Idle Stand"] = 7772892453, 
				["Pose Idle root"] = 7772893941
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6924591468, 
				Idle = 6930660376
			}
		}, 
		Nocturnus = {
			Action = {
				["LMB-1"] = 6999930037, 
				["LMB-2"] = 6999931366, 
				["LMB-3"] = 6999932146, 
				["LMB-4"] = 6999932888, 
				LeashSlash = 6968510181, 
				FlashSlash = 6968512967, 
				Stab = 6968516930, 
				Grab = 6968514367, 
				SwipeUp = 6999600490, 
				SwipeDown = 6999582253, 
				PoseIdle = 8051172224, 
				PoseTransition = 8051125789
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6934448581, 
				Idle = 6934449317
			}
		}, 
		["Demon Lord"] = {
			Action = {
				DevilEyes = 6948655414
			}
		}, 
		Standless = {
			Action = {
				BiteAttempt = 7118590427, 
				BiteSuccess = 7118711342, 
				BiteVictim = 7118710416, 
				StylishSweeps = 7118819267, 
				Taunt = 7118739515, 
				Dodge = 5191300871, 
				GrabAttempt = 7113256345, 
				AsphaltSuccess = 7113253353, 
				AsphaltVictim = 7113252192, 
				DropKick = 7118274633, 
				GunShots = 7117836119, 
				ForwardDash = 10451361960, 
				BackwardDash = 10451359576, 
				LeftDash = 10451363828, 
				RightDash = 10451365211, 
				PoseTransition = 7124468256
			}, 
			Idle = {
				Idle = 7473308966
			}
		}, 
		Whitesnake = {
			Action = {
				["LMB-1"] = 10036899069, 
				["LMB-2"] = 10036901629, 
				["LMB-3"] = 10036907704, 
				["LMB-4"] = 10036912652, 
				Block = 10053550381, 
				PilotUserIdle = 10035919728, 
				PilotUserTransition = 10035917372, 
				PoseTransition = 7816101964, 
				PoseIdle = 7816100125, 
				PilotPoseTransition = 10037143983, 
				PilotPoseIdle = 10037137790, 
				CountTransition = 10105282346, 
				CountIdle = 10105285054, 
				Crucifixion = 8222028942, 
				Barrage = 6307582703, 
				AcidStrikes = 8253153422, 
				RemoteBarrageUser = 8283325994, 
				RemoteBarrage = 8222733093, 
				TargetSleep = 8283607580, 
				TargetSleeping = 8283609530, 
				IllusoryBlow = 10054383820, 
				DomineQuoVadis = 8253822953, 
				DomineQuoVadisPilot = 8254133077, 
				DirectOrder = 9855589080, 
				["Hand Disc"] = 7911757423, 
				DiscInsertion = 10047933669, 
				DiscExtraction = 10048460161, 
				DiscExtractTarget = 10094738678, 
				PalePursuitBarrage = 9955803229, 
				PalePursuitStartup = 10037484628, 
				PalePursuitRun = 9955800110, 
				PalePursuitConfirm = 9955801599, 
				KillerPerception = 10034709631, 
				KillerPerceptionPilot = 10105112285, 
				["RhinocerosBeetle Attack"] = 9955779856, 
				["RhinocerosBeetle Hit"] = 9955782521, 
				["RhinocerosBeetle HitVictim"] = 9955786162, 
				MeltYourHeart = 10053333254, 
				Disguise = 10059245112, 
				PilotForwardDash = 10128375083, 
				PilotBackwardDash = 10128373129, 
				PilotLeftDash = 10128376957, 
				PilotRightDash = 10128378333
			}, 
			Movement = {
				Walk = 10158780189, 
				SummonedWalk = 10158780189, 
				SummonedRun = 7037969480
			}, 
			Idle = {
				StandIdle = 10536859878, 
				Idle = 10074269379
			}
		}, 
		["C-Moon"] = {
			Action = {
				PoseTransition = 8101642840, 
				PoseIdle = 8101642004, 
				Gunshots = 6779300880, 
				Pose = 5340508465, 
				["LMB-1"] = 6761487530, 
				["LMB-2"] = 6761488706, 
				["LMB-3"] = 6761489488, 
				["LMB-4"] = 6761490353, 
				Barrage = 5790894843, 
				Counter = 6907917677, 
				OFFBarrage = 6780083994, 
				Chop = 6769082841, 
				Slam = 7082224490, 
				DiveKick = 6784905848, 
				StrongPunch = 6663831578, 
				["Strong Punch"] = 6663831578, 
				CounterPunch = 6907966579, 
				Uppercut = 6796758526, 
				UppercutStandOff = 6516570355, 
				Jab = 6516570355, 
				Victim = 6819166024, 
				Victim2 = 6819205830, 
				GroundSlam = 6819167773, 
				GroundSlam2 = 6823631691, 
				AAAAA = 6670284770
			}, 
			Movement = v5, 
			Idle = {
				Idle = 7364204477, 
				StandIdle = 6785812733
			}
		}, 
		["C-Moon R"] = {
			Action = {
				PoseTransition = 8101642840, 
				PoseIdle = 8101642004, 
				ArmCrusher = 10629210500, 
				ArmCrusherReaction = 10632044582, 
				Pose = 5340508465, 
				["LMB-1"] = 10517397886, 
				["LMB-2"] = 10517411697, 
				["LMB-3"] = 10517414920, 
				["LMB-4"] = 10517417315, 
				["StandOff-LMB-1"] = 10688396131, 
				["StandOff-LMB-2"] = 10688401326, 
				["StandOff-LMB-3"] = 10688403836, 
				["StandOff-LMB-4"] = 10688406327, 
				Barrage = 10772370938, 
				Counter = 6907917677, 
				OFFBarrage = 6780083994, 
				BrainHemorrhage = 10822557991, 
				BrainHemorrhageReaction = 10822679224, 
				Slam = 7082224490, 
				StrongPunch = 6663831578, 
				CounterPunch = 6907966579, 
				Uppercut = 6796758526, 
				UppercutStandOff = 6516570355, 
				Jab = 6516570355, 
				Victim = 6819166024, 
				Victim2 = 6819205830, 
				GroundSlam = 6819167773, 
				GroundSlam2 = 6823631691, 
				AAAAA = 6670284770, 
				DebrisSlamShort = 10290217893, 
				DebrisSlamLong = 10376964677, 
				BodyMassIndex = 10400927853, 
				BMIVictimHeavy = 10450255583, 
				BMIVictimInversion = 10450263121
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6785812733, 
				Idle = 7364204477
			}
		}, 
		T_CM = {
			Action = {
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				PilotUserIdle = 8219591137, 
				PilotUserTransition = 8219592177, 
				PoseTransition = 7816101964, 
				PoseIdle = 7816100125, 
				Crucifixion = 8222028942, 
				Barrage = 6307582703, 
				AcidStrikes = 8253153422, 
				RemoteBarrageUser = 8283325994, 
				RemoteBarrage = 8222733093, 
				TargetSleep = 8283607580, 
				TargetSleeping = 8283609530, 
				IllusoryBlow = 8253581455, 
				DomineQuoVadis = 8253822953, 
				DomineQuoVadisPilot = 8254133077, 
				["Gravitational Elimination"] = 9430824021, 
				["Gravitational EliminationHit"] = 9430828975, 
				["Gravitational Camera Attempt"] = 9430885384, 
				["Gravitational Camera"] = 9430887589, 
				["Gravitational Victim"] = 9430889658
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6820655855
			}
		}, 
		["Made In Heaven"] = {
			Action = {
				Pose = 8055168044, 
				PoseIdle = 8055170863, 
				EStandOff = 6746357635, 
				QuickJab = 6742538911, 
				["LMB-1"] = 6750197876, 
				["LMB-2"] = 6750195977, 
				["LMB-3"] = 6750197100, 
				["LMB-4"] = 6750197520, 
				["StandOff-LMB-1"] = 6749658606, 
				["StandOff-LMB-2"] = 6749660428, 
				["StandOff-LMB-3"] = 6749662623, 
				["StandOff-LMB-4"] = 6749663398, 
				MiHChop = 6769082841, 
				Conuter = 7045210066, 
				BackDashKnives = 6758894361, 
				DownKnives = 6758927514, 
				PunchBarrage = 6750252452, 
				BurstBarrage = 6751298313, 
				RightPunch = 6754448913, 
				Roll = 5191300871, 
				SF = 5164214146
			}, 
			Movement = {
				TimeAccel = 6630347677, 
				Run = 7037969480, 
				Walk = 6877996750, 
				SummonedRun = 7037969480, 
				SummonedWalk = 6877996750
			}, 
			Idle = {
				StandIdle = 7367667043, 
				Idle = 7367593771
			}
		}, 
		T_MIH = {
			Action = {
				["StandOff-LMB-1"] = 9543697950, 
				["StandOff-LMB-2"] = 9543700963, 
				["StandOff-LMB-3"] = 9543702537, 
				["StandOff-LMB-4"] = 9543704330, 
				["Behind You!"] = 9536216452
			}, 
			Movement = {
				TimeAccel = 6630347677, 
				Run = 7037969480, 
				Walk = 6877996750, 
				SummonedRun = 7037969480, 
				SummonedWalk = 6877996750
			}, 
			Idle = {
				StandIdle = 7367667043, 
				Idle = 7367593771
			}
		}, 
		DOG = {
			Action = {
				Summon = 6774704354, 
				StrongPunch = 6774704354
			}
		}, 
		Shinigami = {
			Action = {
				AttackPose = 5922281900, 
				BlashFire = 4554563880, 
				HealBarrage = 5146177853, 
				Chop = 5340465483, 
				HealOverwrite = 5150190585, 
				Kick = 5340460049, 
				StrongerStrongPunch = 5340532395, 
				Idle = 5340484318, 
				LeftPunch = 5143376290, 
				Overwrite = 5150170356, 
				Pose = 5269135562, 
				PunchBarrage = 5790894843, 
				RightPunch = 5143367853, 
				Roll = 5191300871, 
				SF = 5164214146, 
				Slam = 5150294247, 
				StandJump = 5889373753, 
				StrongPunch = 6663831578, 
				Timestop = 5915276164, 
				AttackPoseLooped = 6568461661, 
				AttackPoseTransition = 6568465045
			}
		}, 
		CakePlatinum = {
			Action = {
				AttackPose = 5922281900, 
				BlashFire = 4554563880, 
				SelfHeal = 5146177853, 
				Idle = 5778922246, 
				LeftPunch = 5143376290, 
				Overwrite = 5150170356, 
				Pose = 5303113036, 
				PunchBarrage = 5790894843, 
				RightPunch = 5143367853, 
				Roll = 5191300871, 
				SF = 5164214146, 
				Slam = 5150294247, 
				StandJump = 5889373753, 
				StrongPunch = 5965700661, 
				Timestop = 5915276164, 
				AttackPoseLooped = 6568461661, 
				AttackPoseTransition = 6568465045
			}
		}, 
		AngelicPlatinum = {
			Action = {
				AttackPose = 5922281900, 
				BlashFire = 4554563880, 
				Drill = 5263173421, 
				SelfHeal = 5146177853, 
				Idle = 5778922246, 
				LeftPunch = 5143376290, 
				Overwrite = 5150170356, 
				Pose = 5143357677, 
				PunchBarrage = 5790894843, 
				RightPunch = 5143367853, 
				Roll = 5191300871, 
				SF = 5164214146, 
				Slam = 5150294247, 
				StandJump = 5889373753, 
				StrongPunch = 5965700661, 
				Timestop = 5146277255, 
				animfly = 5508281814, 
				AttackPoseLooped = 6568461661, 
				AttackPoseTransition = 6568465045
			}
		}, 
		Gojo = {
			Action = {
				TeleportationKick = 6490852120, 
				["Air Palm"] = 10571329944, 
				TeleportLand = 6920495191, 
				KickStarter = 10628205744, 
				["Hollow Purple"] = 7005477388, 
				AttackPose = 6307839827, 
				BlueAmplificationThrow = 6901464282, 
				Snap = 6901466200, 
				DomainExpansion = 6539490566, 
				Pose = 6544470612, 
				["LMB-1"] = 10571338890, 
				["LMB-2"] = 10571341987, 
				["LMB-3"] = 10571344976, 
				["LMB-4"] = 10571348040, 
				AOE = 10438583499, 
				ReversalRed = 7026655617, 
				GrabAttempt = 6700676341, 
				Beatdown = 6909885789, 
				BeatdownVictim = 6909903316, 
				GrabFail = 9390593282, 
				DEActivate = 9856849601, 
				DECutscene = 9510613580, 
				DECutsceneVictim = 9510620622, 
				DECutsceneCamera = 9511808330, 
				AirPalmRecoil = 10631991742
			}, 
			Idle = {
				Idle = 7317390939
			}
		}, 
		Gojo_R = {
			Action = {
				TeleportationKick = 6490852120, 
				["Air Palm"] = 10571329944, 
				TeleportLand = 6920495191, 
				KickStarter = 10628205744, 
				["Hollow Purple"] = 7005477388, 
				AttackPose = 6307839827, 
				BlueAmplificationThrow = 6901464282, 
				Snap = 6901466200, 
				DomainExpansion = 6539490566, 
				Pose = 6544470612, 
				["LMB-1"] = 10571338890, 
				["LMB-2"] = 10571341987, 
				["LMB-3"] = 10571344976, 
				["LMB-4"] = 10571348040, 
				AOE = 10438583499, 
				ReversalRed = 7026655617, 
				GrabAttempt = 6700676341, 
				Beatdown = 6909885789, 
				BeatdownVictim = 6909903316, 
				GrabFail = 9390593282, 
				DEActivate = 9856849601, 
				DECutscene = 9510613580, 
				DECutsceneVictim = 9510620622, 
				DECutsceneCamera = 9511808330, 
				AirPalmRecoil = 10631991742, 
				Grab = 11110729280, 
				Throw = 11110730939, 
				ThrowVictim = 11110732132
			}, 
			Idle = {
				Idle = 7317390939
			}
		}, 
		["King Crimson"] = {
			Action = {
				["LMB-1"] = 6761487530, 
				["LMB-2"] = 6761488706, 
				["LMB-3"] = 6761489488, 
				["LMB-4"] = 6761490353, 
				["Doppio Slam"] = 6981444373, 
				["Eye Jab"] = 6972331642, 
				["Burst Barrage"] = 6972374480, 
				["Scalpel Throw"] = 7348496687, 
				Donut = 6900047501, 
				["Donut Hit"] = 6900049658, 
				["Donut Victim"] = 6900049015, 
				["Arm Chop Startup"] = 6923711407, 
				["Arm Chop Hit"] = 6905345859, 
				Counter = 7025040286, 
				["Counter Victim"] = 7025049036, 
				["Take Off Shirt"] = 6938334709, 
				["Time Erase"] = 6789950709, 
				Barrage = 6307582703, 
				Chop = 6761487530, 
				Follow = 6905345859, 
				Pose = 7507978152, 
				PoseTransition = 7507993550
			}, 
			Movement = {
				Walk = 7339784680, 
				SummonedWalk = 7339784680, 
				Run = 7037969480, 
				SummonedRun = 7037969480
			}, 
			Idle = {
				Idle = 7193291733, 
				StandIdle = 7193259256
			}
		}, 
		["The World"] = {
			Action = {
				Barrage = 6307582703, 
				Donut = 6700246793, 
				TS = 7070692651, 
				GrabThrow = 6466281270, 
				ThrowGrab = 6466283071, 
				Checkmate = 6746021275, 
				GroundSlam = 6754411814, 
				SignSlam = 6449239412, 
				WRY = 6733919900, 
				Kick = 6238231437, 
				TeleportPose = 6313231576, 
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				AttackPose = 6307839827, 
				Tandem = 6313729731, 
				DashAttackPose = 6316519347, 
				RoundhouseKick = 6328384081, 
				SlamPunch = 6516569709, 
				BloodSuckAttempt = 6753687790, 
				AerialChop = 6745673036, 
				JosephKnife = 6316893120, 
				Lunge = 6313729731, 
				KickBarrage = 10140174898, 
				RoadRoller = 7097331918, 
				RoadRollerAnim = 7097331918, 
				PoseTransition = 10528708480, 
				PoseIdle = 10528723562
			}, 
			Movement = v5, 
			Idle = {
				Idle = 10548864046, 
				StandIdle = 10548855334
			}
		}, 
		["Killer Queen"] = {
			Action = {
				Barrage = 6420707857, 
				HeavyPunch = 6330983021, 
				["Primary Bomb"] = 6421362019, 
				["Yen Throw"] = 6567517933, 
				Detonate = 6421361576, 
				LMB = 6577748776, 
				["LMB-1"] = 6761487530, 
				["LMB-2"] = 6761488706, 
				["LMB-3"] = 6761489488, 
				["LMB-4"] = 6761490353, 
				["Bubble Bomb"] = 6590183065, 
				["Punch Bomb"] = 6594526758, 
				Uppercut = 6594543037, 
				["Face Grab"] = 6700676341, 
				["Third Bomb"] = 6690947113, 
				["BTD Pose"] = 6694883914, 
				["BTD Activate"] = 6693526640, 
				["BTD Loop"] = 6693530588, 
				VPIdle = 6682523681, 
				VPDetonate = 6685427570, 
				["Secondary Bomb"] = 6738925318, 
				Pose = 7508212350, 
				PoseTransition = 7508188405
			}, 
			Movement = v5, 
			Idle = {
				Idle = 6708778082, 
				StandIdle = 6820065461
			}
		}, 
		KQ_R = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				["StandOff-LMB-1"] = 11127865908, 
				["StandOff-LMB-2"] = 11127868260, 
				["StandOff-LMB-3"] = 11127869614, 
				["StandOff-LMB-4"] = 11127870798, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				Grab = 10906128504, 
				Throw = 10906131878, 
				ThrowVictim = 10906132668, 
				["Flying Uppercut"] = 10840806004, 
				["Primary Bomb"] = 10843864386, 
				Detonate1 = 10856506805, 
				Detonate2 = 10856508771, 
				["Stand Restrain Startup"] = 11165590102, 
				["Stand Restrain User"] = 10848564777, 
				["Stand Restrain Victim"] = 10848566966, 
				["Stand Restrain Victim Loop"] = 10848569219, 
				["Stand Restrain User Loop"] = 10848571714, 
				Explode = 10855711598, 
				CautiousStrike = 10857148827, 
				["Plant Bomb"] = 10855748127, 
				["Kick Away"] = 10897756070, 
				["Coin Toss"] = 10857145963, 
				PoseIdle = 7508212350, 
				PoseTransition = 7508188405, 
				DonutStartup = 10898048721, 
				DonutUser = 10898039552, 
				DonutVictim = 10898041509, 
				["Face Slam Startup"] = 10912968659, 
				["Face Slam Victim"] = 10912971104, 
				["Face Slam User"] = 10912975539, 
				["Face Slam Camera"] = 10912977180, 
				["SHA Plant"] = 10938569205, 
				["Quadruple Bomb Finish"] = 10944261635, 
				["Quadruple Bomb Finish User"] = 10944263399, 
				["Quadruple Bomb Finish Victim"] = 10944265280, 
				["Quick Plant"] = 11126752547, 
				["Quick Plant User"] = 11126755703, 
				["Quick Plant Victim"] = 11126757411, 
				["Quote-1"] = 10976760361, 
				["Quote-2"] = 10976761195, 
				["Quote-3"] = 10976763020
			}, 
			Movement = {
				Walk = 10856503017, 
				Run = 10856500879, 
				SummonedWalk = 10856503017, 
				SummonedRun = 10856500879, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 10636699829, 
				Idle = 10842851957
			}
		}, 
		["Senator Armstrong"] = {
			Action = {}, 
			Movement = {}, 
			Idle = {}
		}, 
		["Phantom Queen"] = {
			Action = {
				Barrage = 6420707857, 
				HeavyPunch = 6330983021, 
				["Primary Bomb"] = 6421362019, 
				["Yen Throw"] = 6567517933, 
				Detonate = 6421361576, 
				LMB = 6577748776, 
				["LMB-1"] = 6761487530, 
				["LMB-2"] = 6761488706, 
				["LMB-3"] = 6761489488, 
				["LMB-4"] = 6761490353, 
				["Bubble Bomb"] = 6590183065, 
				["Punch Bomb"] = 6594526758, 
				Uppercut = 6594543037, 
				["Face Grab"] = 6700676341, 
				["Third Bomb"] = 6690947113, 
				["BTD Pose"] = 6694883914, 
				["BTD Activate"] = 6693526640, 
				["BTD Loop"] = 6693530588, 
				VPIdle = 6682523681, 
				VPDetonate = 6685427570, 
				["Secondary Bomb"] = 6738925318, 
				Pose = 7508212350, 
				PoseTransition = 7508188405
			}, 
			Idle = {
				StandIdle = 8054510853
			}
		}, 
		["Creeper Queen"] = {
			Action = {
				Barrage = 6420707857, 
				HeavyPunch = 6330983021, 
				["Primary Bomb"] = 6421362019, 
				["Yen Throw"] = 6567517933, 
				Detonate = 6421361576, 
				LMB = 6577748776, 
				["LMB-1"] = 6761487530, 
				["LMB-2"] = 6761488706, 
				["LMB-3"] = 6761489488, 
				["LMB-4"] = 6761490353, 
				["Bubble Bomb"] = 6590183065, 
				["Punch Bomb"] = 6594526758, 
				Uppercut = 6594543037, 
				["Face Grab"] = 6700676341, 
				["Third Bomb"] = 6690947113, 
				["BTD Pose"] = 6694883914, 
				["BTD Activate"] = 6693526640, 
				["BTD Loop"] = 6693530588, 
				VPIdle = 6682523681, 
				VPDetonate = 6685427570, 
				["Secondary Bomb"] = 6738925318, 
				Pose = 7508212350, 
				PoseTransition = 7508188405
			}, 
			Idle = {
				StandIdle = 6820065461
			}
		}, 
		["Uber Oni"] = {
			Action = {
				Rampage = 6792665091, 
				DemonStep = 6981841742, 
				ConsumingFlames = 6793391689, 
				Misogi = 6793551810, 
				Flip1 = 6794016801, 
				Flip2 = 6800964305, 
				RisingDragon = 6801013416, 
				LegBreaker = 6801228703
			}
		}, 
		Omnitrix = {
			Action = {
				Select = 6755594110, 
				Pyrokinesis = 6768194987, 
				["Fireball Generation"] = 6771876128, 
				["Fire Punch"] = 6771876128, 
				["Quick Swing"] = 6796338854, 
				["Vortex Attempt"] = 6806219463, 
				["Vortex Start"] = 6811937143, 
				["Vortex End"] = 6812069893, 
				Vortex = 6806224461, 
				["DiamondHead Punch"] = 7123660390, 
				["DiamondHead Jab"] = 7123666255, 
				Crystallokinesis = 7065705093, 
				PoseIdle = 7772848382, 
				PoseTransition = 7772884995
			}, 
			Idle = {
				Idle = 6630333014, 
				HeatBlastIdle = 7062472761, 
				DiamondHeadIdle = 7065699280, 
				XLR8Idle = 7062736137
			}
		}, 
		["Omnitrix Rewrite"] = {
			Action = {
				Select = 6755594110, 
				Pyrokinesis = 6768194987, 
				["Fireball Generation"] = 6771876128, 
				["Fire Punch"] = 6771876128, 
				["Quick Swing"] = 6796338854, 
				["Vortex Attempt"] = 6806219463, 
				["Vortex Start"] = 6811937143, 
				["Vortex End"] = 6812069893, 
				Vortex = 6806224461, 
				HeatBlastIdle = 7062472761, 
				XLR8Idle = 7062736137, 
				DiamondHeadIdle = 7065699280, 
				["DiamondHead Punch"] = 7123660390, 
				["DiamondHead Jab"] = 7123666255, 
				Crystallokinesis = 7065705093, 
				PoseIdle = 7772848382, 
				PoseTransition = 7772884995
			}
		}, 
		["Star Platinum"] = {
			Action = {
				Barrage = 6331004626, 
				HeavyPunch = 6663831578, 
				StarFingerDrawIn = 6443690567, 
				AttackPoseTransition = 6568465045, 
				AttackPoseLooped = 6568461661, 
				StarFingerCharge = 6443694721, 
				StarFingerFire = 6444603026, 
				Drink = 6473199424, 
				GunFire = 6881684286, 
				GroundSlam = 6647782995, 
				TandemGrab = 6501104935, 
				TandemBarrage = 6501111552, 
				GunFireWithoutArm = 7364356745, 
				CounterPose = 6517571218, 
				CounterPoseTransition = 6517565588, 
				StarSuck = 6513647737, 
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				StarSucking = 6513650958, 
				Pose = 10179278620, 
				PoseTransition = 10179275232, 
				MetalRod = 6513576048, 
				KickBarrage = 6687607030, 
				Timestop = 6933820161, 
				GrabAttempt = 7198758483, 
				GrabSuccess = 7198762633, 
				GrabVictim = 7198764309
			}, 
			Movement = {
				Walk = 7386802270, 
				Run = 7331835388, 
				SummonedWalk = 7386802270, 
				SummonedRun = 7331835388
			}, 
			Idle = {
				StandIdle = 7176839231, 
				Idle = 7339780665
			}
		}, 
		SP_R = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				["StandOff-LMB-1"] = 11371980872, 
				["StandOff-LMB-2"] = 11371981731, 
				["StandOff-LMB-3"] = 11371982707, 
				["StandOff-LMB-4"] = 11371983463, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				Grab = 10906128504, 
				Throw = 10906131878, 
				ThrowVictim = 10906132668, 
				["Star Breaker"] = 10603603515, 
				["Star Finger"] = 10604735658, 
				["Evil Spirit"] = 10824269024, 
				["Inhale Startup"] = 10627518398, 
				["Inhale Looped"] = 10627522140, 
				Timestop = 10619893836, 
				["Ora Slam"] = 10604996457, 
				AttackPoseTransition = 6568465045, 
				AttackPoseLooped = 6568461661, 
				Drink = 10615944161, 
				GroundSlam = 6647782995, 
				["Brute Force Attempt"] = 10629787650, 
				["Brute Force Hit"] = 10629797095, 
				["Brute Force Victim"] = 10629800082, 
				Beatdown_Startup = 11320522791, 
				Beatdown_Camera = 11320552981, 
				Beatdown_Victim = 11320554701, 
				Beatdown_UserSuccessful = 11320555645, 
				Lock_Kick = 11352124336, 
				["Grab Slam Startup"] = 11352494189, 
				["Grab Slam User"] = 11352496815, 
				["Grab Slam Victim"] = 11352499254, 
				PoseIdle = 10179278620, 
				PoseTransition = 10179275232, 
				["Quote-1"] = 10976621202, 
				["Quote-2"] = 10976662892, 
				["Quote-3"] = 10976663588
			}, 
			Movement = {
				Walk = 10629833287, 
				Run = 7331835388, 
				SummonedWalk = 10629833287, 
				SummonedRun = 7331835388, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 10636699829, 
				Idle = 10636697572
			}
		}, 
		KC_R = {
			Action = {
				["LMB-1"] = 11101062240, 
				["LMB-2"] = 11101070887, 
				["LMB-3"] = 11101075126, 
				["LMB-4"] = 11101078322, 
				["StandOff-LMB-1"] = 11203522877, 
				["StandOff-LMB-2"] = 11203526095, 
				["StandOff-LMB-3"] = 11203534927, 
				["StandOff-LMB-4"] = 11203540441, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				Grab = 10907328566, 
				Throw = 10907329255, 
				ThrowVictim = 10907329938, 
				CleavingStrikes = 10913480978, 
				Chop = 10913373242, 
				ImpaleAttempt = 10913665434, 
				Impale = 10913666748, 
				TargetImpaled = 10913667309, 
				GroundSlam = 10938293800, 
				DownwardStrike = 11005558877, 
				SuddenBlowStartup = 10938760715, 
				SuddenBlowLoop = 10938762256, 
				SuddenBlowAttack = 10938763439, 
				SuddenImpale = 6900049658, 
				SuddenImpaleVictim = 6900049015, 
				ScalpelThrow = 10938296287, 
				Epitaph = 10938395302, 
				Counter = 7025040286, 
				CounterVictim = 7025049036, 
				FierceGrab = 10938492839, 
				FierceThrow = 10938497083, 
				FierceThrowVictim = 10938498905, 
				TimeErase = 11108625453, 
				PoseIdle = 7507978152, 
				PoseTransition = 7507993550
			}, 
			Movement = {
				Walk = 10907213293, 
				SummonedWalk = 10907213293, 
				Run = 10914799131, 
				SummonedRun = 10914799131, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				Idle = 10907211857, 
				StandIdle = 10907242780
			}
		}, 
		WS_R = {
			Action = {
				["LMB-1"] = 10036899069, 
				["LMB-2"] = 10036901629, 
				["LMB-3"] = 10036907704, 
				["LMB-4"] = 10036912652, 
				["StandOff-LMB-1"] = 10688396131, 
				["StandOff-LMB-2"] = 10688401326, 
				["StandOff-LMB-3"] = 10688403836, 
				["StandOff-LMB-4"] = 10688406327, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				AcidStrikes = 11370443258, 
				RemoteBarrageUser = 8283325994, 
				RemoteBarrage = 8222733093, 
				DomineQuoVadis = 8253822953, 
				DomineQuoVadisPilot = 8254133077, 
				KneeSlamStartup = 10912968659, 
				KneeSlam = 11289217670, 
				KneeSlamVictim = 11289268101, 
				Crucifixion = 8222028942, 
				KillerPerception = 10034709631, 
				KillerPerceptionPilot = 10105112285, 
				IllusoryBlow = 10054383820, 
				RhinocerosBeetleStartup = 9955779856, 
				RhinocerosBeetle = 9955782521, 
				RhinocerosBeetleVictim = 9955786162, 
				DirectOrder = 9855589080, 
				HandDisc = 7911757423, 
				MeltYourHeart = 10053333254, 
				TargetSleep = 8283607580, 
				TargetSleeping = 8283609530, 
				DiscExtraction = 10048460161, 
				DiscExtractTarget = 10094738678, 
				DiscInsertion = 10047933669, 
				PalePursuitBarrage = 9955803229, 
				PalePursuitStartup = 10037484628, 
				PalePursuitRun = 9955800110, 
				PalePursuitConfirm = 9955801599, 
				Disguise = 10059245112, 
				CountTransition = 10105282346, 
				CountIdle = 10105285054, 
				PilotUserIdle = 10035919728, 
				PilotUserTransition = 10035917372, 
				PoseTransition = 7816101964, 
				PoseIdle = 7816100125, 
				PilotPoseTransition = 10037143983, 
				PilotPoseIdle = 10037137790
			}, 
			Movement = {
				Walk = 10158780189, 
				SummonedWalk = 10158780189, 
				SummonedRun = 7037969480, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289, 
				PilotForwardDash = 10128375083, 
				PilotBackwardDash = 10128373129, 
				PilotLeftDash = 10128376957, 
				PilotRightDash = 10128378333
			}, 
			Idle = {
				StandIdle = 10536859878, 
				Idle = 10074269379
			}
		}, 
		CM_R = {
			Action = {
				["LMB-1"] = 11063407023, 
				["LMB-2"] = 11063410729, 
				["LMB-3"] = 11063412797, 
				["LMB-4"] = 11063414925, 
				["StandOff-LMB-1"] = 10688396131, 
				["StandOff-LMB-2"] = 10688401326, 
				["StandOff-LMB-3"] = 10688403836, 
				["StandOff-LMB-4"] = 10688406327, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 11064727600, 
				Barrage = 11064717857, 
				BarrageFinisher = 11064723359, 
				BarrageClashEnd = 10839831781, 
				CenterOfGravity = 10999442929, 
				Grab = 10907328566, 
				Throw = 10907329255, 
				ThrowVictim = 10907329938, 
				InversionStrike = 11092487307, 
				InversionStrikeVictim = 10981072367, 
				HeartInversion = 11092518454, 
				HeartInversionVictim = 10981148112, 
				ArmCrusher = 10629210500, 
				ArmCrusherVictim = 10632044582, 
				SingularityPoint = 11092535961, 
				OnlyOnePunch = 11062207096, 
				OnlyOnePunchAttack = 11062210242, 
				OnlyOnePunchVictim = 11062212505, 
				GroundSlam = 10981318242, 
				DebrisShotgun = 10981321823, 
				PalmKinesis = 11092566315, 
				EliminationStartup = 11231006296, 
				EliminationStartupVictim = 11231028815, 
				Elimination = 11231118645, 
				EliminationVictim = 11231140458, 
				EliminationCamera = 11231241727, 
				GravityShift = 11237697351, 
				PilotUserIdle = 11100475650, 
				PilotUserTransition = 11100473471, 
				PilotForwardDash = 10128375083, 
				PilotBackwardDash = 10128373129, 
				PilotLeftDash = 10128376957, 
				PilotRightDash = 10128378333, 
				CountTransition = 10105282346, 
				CountIdle = 10105285054, 
				PoseIdle = 8101642004, 
				PoseTransition = 8101642840, 
				["Quote-1"] = 11106373775, 
				["Quote-2"] = 11106382126, 
				["Quote-3"] = 11106383700, 
				Float = 11265008044
			}, 
			Movement = {
				Walk = 10998529485, 
				SummonedWalk = 10998529485, 
				Run = 10914799131, 
				SummonedRun = 10914799131, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 10998520770, 
				Idle = 10998515521
			}
		}, 
		MIH_R = {
			Action = {
				["StandOff-LMB-1"] = 10688396131, 
				["StandOff-LMB-2"] = 10688401326, 
				["StandOff-LMB-3"] = 10688403836, 
				["StandOff-LMB-4"] = 10688406327, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 11064727600, 
				Barrage = 11064717857, 
				BarrageFinisher = 11064723359, 
				BarrageClashEnd = 10839831781, 
				Grab = 10907328566, 
				Throw = 10907329255, 
				ThrowVictim = 10907329938
			}, 
			Movement = {
				Walk = 10998529485, 
				SummonedWalk = 10998529485, 
				Run = 10914799131, 
				SummonedRun = 10914799131, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 10998520770, 
				Idle = 10998515521
			}
		}, 
		SP_CR = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				Block = 10808688837, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 10002462639, 
				Barrage = 10603510761, 
				BarrageFinisher = 10603516376, 
				StarBreaker = 10603603515, 
				Grab = 9955779856, 
				Grabbed = 9955782521, 
				GrabbedVictim = 9955786162
			}, 
			Movement = {
				Walk = 10629833287, 
				Run = 7331835388, 
				SummonedWalk = 10629833287, 
				SummonedRun = 7331835388
			}, 
			Idle = {
				StandIdle = 10636699829, 
				Idle = 10636697572
			}
		}, 
		["Star Platinum: The World"] = {
			Action = {
				Barrage = 6331004626, 
				AttackPoseTransition = 6568465045, 
				AttackPoseLooped = 6568461661, 
				Timestop = 6575563592, 
				TimestopStandOn = 6590354245, 
				HeavyPunch = 6663831578, 
				GroundSlam = 6647782995, 
				KickBarrage = 6687607030, 
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				Pose = 6582571947, 
				PoseTransition = 6582573647, 
				Bearing = 6736397929, 
				JabDash = 6589691798, 
				Jab = 6773671645, 
				Crush = 6768572898, 
				Resolve = 7405890993, 
				ChinCrusher = 10517708934, 
				LiverShot = 10518423859, 
				BeatdownPunch = 10446639889, 
				BurstTimestop = 10518646803
			}, 
			Movement = {
				Walk = 7386804902, 
				Run = 7331835388, 
				SummonedWalk = 7386804902, 
				SummonedRun = 7331835388
			}, 
			Idle = {
				Idle = 6645554296, 
				StandIdle = 7176811862
			}
		}, 
		Inker = {
			Action = {
				AttackPose = 6600255288, 
				AttackPoseTransition = 6568465045, 
				AttackPoseLooped = 6568461661, 
				Barrage = 6421231197, 
				HeavyPunch = 6330983021, 
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				Pose = 6742642203, 
				glide = 7045700729, 
				Timestop = 6933820161, 
				PoseTransition = 6742642896, 
				RMove = 7040077713, 
				Ultimate = 7040449256, 
				["S-Summon"] = 8961582641, 
				["S-Idle"] = 8961586691, 
				["S-Move"] = 8961596846, 
				["S-Roar"] = 9054635954, 
				["S-Slash"] = 8961608372, 
				["S-Desummon"] = 8961612022
			}, 
			Idle = {
				StandIdle = 6421260216
			}
		}, 
		["\206\180:for the DELTA"] = {
			Action = {
				FreezePlayer = 6333146548, 
				OnKnees = 6334076639, 
				Shockwave = 6290528162, 
				StandSummon = 6333716743, 
				TurnBackTime = 6333151996, 
				PoseStart = 6414190677, 
				PoseEnd = 6414193632, 
				PoseLoop = 6414352667
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6333137550
			}
		}, 
		DTWHV = {
			Action = {
				AttackPose = 6600255288, 
				Barrage = 6331004626, 
				Cutscene = 7037887987, 
				Gasoline = 5697356924, 
				Kick = 5224441129, 
				KnifeAnim = 7195050558, 
				UrgentTS = 6612929603, 
				Pose1 = 5730215005, 
				GunFire = 6501360764, 
				Pose2 = 5730215005, 
				PunchBarrage = 5704092469, 
				StandJump = 5889373753, 
				HeavyPunch = 6663831578, 
				Timestop = 7060238054, 
				Sit = 5718959564, 
				WireThrow = 6649402629, 
				HeavyMuda = 6768306270, 
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6606063246
			}
		}, 
		TWHV = {
			Action = {
				AttackPose = 6600255288, 
				Barrage = 6331004626, 
				Cutscene = 7037887987, 
				Gasoline = 5697356924, 
				Kick = 5224441129, 
				KnifeAnim = 7195050558, 
				UrgentTS = 6612929603, 
				Pose1 = 5730215005, 
				GunFire = 6501360764, 
				Pose2 = 5730215005, 
				PunchBarrage = 5704092469, 
				StandJump = 5889373753, 
				HeavyPunch = 6663831578, 
				Timestop = 7060238054, 
				Sit = 5718959564, 
				WireThrow = 6649402629, 
				HeavyMuda = 6768306270, 
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666, 
				PoseTransition = 8062693425, 
				PoseIdle = 8062689014
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 6606063246, 
				Idle = 6645559257
			}
		}, 
		TWHV_R = {
			Action = {
				Timestop = 0, 
				MeTime = 0, 
				GasolineDouse = 0, 
				Matchsticks = 0, 
				UserUnleash = 11115698996, 
				NeckSnap_Startup = 11158572027, 
				NeckSnap_FollowUp_User = 11158575954, 
				NeckSnap_FollowUp_Victim = 11158578424, 
				FlourishKnives = 11191115479, 
				FlourishKnivesLoop = 11191121324, 
				ThrowKnives = 11191129573, 
				RevolverFire = 10900013938, 
				RevolverFire2 = 11102588253, 
				TWHVBackshot = 11102592463, 
				TWHVBackshot2 = 11102594037, 
				VictimPowderFire = 11102596215, 
				FlashbangToss = 10672569011, 
				VictimBlinded = 0, 
				ArmChop = 11116663362, 
				TripleChop = 0, 
				["Body Blow"] = 10905193306, 
				VictimWinded = 0, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				["LMB-1"] = 10899679325, 
				["LMB-2"] = 10899681628, 
				["LMB-3"] = 10899683751, 
				["LMB-4"] = 10899685767, 
				["StandOff-LMB-1"] = 10856902374, 
				["StandOff-LMB-2"] = 10856903521, 
				["StandOff-LMB-3"] = 10856904632, 
				["StandOff-LMB-4"] = 10856905614
			}, 
			Idle = {
				Idle = 10657388898, 
				StandIdle = 10657384866
			}, 
			Movement = {
				Walk = 10663962417, 
				Run = 10657396383, 
				SummonedRun = 10657396383, 
				SummonedWalk = 10663962417
			}
		}, 
		Crystallized = {
			Action = {
				Ability = 5484256995, 
				Barrage = 5483406546, 
				Block = 5495710819, 
				Dash = 5561572402, 
				Summon = 5487400100, 
				Pose = 5484111490, 
				Slam = 5487446782, 
				StrongPunch = 5482915300, 
				Punch1 = 6647874978, 
				Punch2 = 6647876817, 
				RaiseCrystals = 6648048241, 
				CrystalDash = 6673365250, 
				StandJump = 6673515754
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 5561569807
			}
		}, 
		["Nuclear Star"] = {
			Action = {
				Ability = 5484256995, 
				Barrage = 5483406546, 
				Block = 5495710819, 
				Dash = 5561572402, 
				Summon = 5487400100, 
				Pose = 5484111490, 
				Slam = 5487446782, 
				StrongPunch = 5482915300, 
				Punch1 = 6647874978, 
				Punch2 = 6647876817, 
				RaiseCrystals = 6648048241, 
				CrystalDash = 6673365250, 
				StandJump = 6673515754
			}, 
			Movement = v5, 
			Idle = {
				StandIdle = 5561569807
			}
		}, 
		Sans = {
			Action = {
				Switch = 6745399620, 
				["Bone Guard"] = 7272561672, 
				["LMB-1"] = 7298024103, 
				["LMB-2"] = 7298030784, 
				["LMB-3"] = 7298037078, 
				["LMB-4"] = 7298041852, 
				Teleport = 7298009816, 
				Bait = 6888629358, 
				BoneLaunch = 6861728070, 
				PoseTransition = 7782503795, 
				PoseIdle = 7782502700
			}, 
			Movement = {
				Walk = 7272215843, 
				Run = 7272215238
			}, 
			Idle = {
				Idle = 7272213387
			}
		}, 
		SINKING = {
			Idle = {
				StandIdle = 6774740934
			}
		}, 
		ShadowDio = {
			Action = {
				Jab = 5743143026, 
				Block = 6884411469, 
				["Crawl Jab"] = 5744018959, 
				["Air High Kick"] = 5745210729, 
				["High Kick"] = 5743435734, 
				Swipe = 5743637619, 
				["Crawl Swipe"] = 5744536754, 
				["Knife Barrage"] = 6877202553, 
				["Stand Uppercut"] = 5814791131, 
				Timestop = 5743687667, 
				Uppercut = 5744251865, 
				["Stand Punishment"] = 6883716199, 
				["User Punishment"] = 6884146636, 
				["Punishment Taunt"] = 6884166974, 
				Counter = 5808743686, 
				Crouch = 5743942990, 
				["Space Ripper"] = 6890349160, 
				["Blood Suck Attempt"] = 7365253855, 
				["Stand Strike"] = 10501998179, 
				ShadowPoseTransition = 7816711555, 
				ShadowPoseIdle = 7816710198, 
				Summon = 8083279582, 
				TeleportPose = 10513224024
			}, 
			Movement = {
				Walk = 5743812382, 
				Run = 7037969480, 
				CrouchWalk = 5743942990, 
				CrouchRun = 5743942990
			}, 
			Idle = {
				Idle = 5743161197, 
				ShadowStandIdle = 8083281888
			}
		}, 
		["S/TW"] = {
			Action = {
				["LMB-1"] = 6579514138, 
				["LMB-2"] = 6579516941, 
				["LMB-3"] = 6579518209, 
				["LMB-4"] = 6579519666
			}, 
			Movement = {
				Walk = 5743812382, 
				Run = 7037969480, 
				SummonedWalk = 5743812382, 
				SummonedRun = 7037969480
			}, 
			Idle = {
				Idle = 10115525271, 
				StandIdle = 10115522627
			}
		}, 
		Reaper = {
			Action = {
				PoseTransition = 7782353441, 
				PoseIdle = 7782352049, 
				["Dimension Rift"] = 6893035303, 
				Wither = 6901716358, 
				Point = 6901643537, 
				["Soul Consumption"] = 6904737035, 
				Block = 6896881487, 
				Frenzy = 6910492396
			}, 
			Movement = {
				Run = 7324808743, 
				Walk = 7324807629
			}, 
			Idle = {
				Idle = 7324806225
			}
		}, 
		["Gold Experience"] = {
			Action = {
				["LMB-1"] = 8479407906, 
				["LMB-2"] = 8479409142, 
				["LMB-3"] = 8479410619, 
				["LMB-4"] = 8479412145, 
				Barrage = 6331004626, 
				HeavyPunch = 7189349499, 
				HeavyKick = 8028012564, 
				RootsStance = 7883668239, 
				RootsRelease = 7883670789, 
				CreateFrog = 8044771960, 
				ConsAttacksUse = 7911757423, 
				ConsAttackCombo = 8489433396, 
				ConsAttackVictim = 8011467457, 
				RestrainUse = 7923267037, 
				RestrainHit = 7923271243, 
				RestrainVictim = 7923273888, 
				Vines = 8075486934, 
				TreeSlam = 8127057861, 
				["Berserk Senses Startup"] = 8378668637, 
				["Berserk Senses Hit"] = 8378670324, 
				["Berserk Senses Camera"] = 8378666695, 
				["Berserk Senses Victim"] = 8378672813, 
				HealOther = 6878291078, 
				SelfHeal = 8027965306, 
				PoseIdle = 10367143160, 
				PoseTransition = 10367140898
			}, 
			Movement = {
				Sit = 5718978019, 
				SummonedRun = 7037969480, 
				SummonedWalk = 6707573199
			}, 
			Idle = {
				Idle = 7193377883, 
				StandIdle = 7193350520
			}
		}, 
		Broly = {
			Action = {
				PoseTransition = 7772902250, 
				Pose = 7772904787, 
				HeavyBlowAttempt = 7454617308, 
				HeavyBlowLoop = 7454620401, 
				ChargeLoop = 7454624282, 
				ChargeEnd = 7454627033, 
				EraserAttempt = 7454630594, 
				EraserBlow = 7454635736, 
				OmegastormWindup = 7454638551, 
				OmegastormLoop = 7454642789, 
				OmegastormEnd = 7454646738, 
				PulverizerAttempt = 7458023010, 
				Pulverizer = 7458025881, 
				GiganticBreath = 7500776853, 
				EraserBall = 7508685914, 
				PlanetCrusher = 7510053489
			}, 
			Movement = {
				Run = 7505927467, 
				Walk = 7505925623
			}, 
			Idle = {
				Idle = 7505893429
			}
		}, 
		["Goku (Rewrite)"] = {
			Action = {
				["LMB-1"] = 10447330139, 
				["LMB-2"] = 10447335715, 
				["LMB-3"] = 10447337080, 
				["LMB-4"] = 10447338237, 
				Kiai = 8995536447, 
				["Kamehameha Start"] = 9000242051, 
				["Kamehameha Loop"] = 9000243142, 
				["Kamehameha Fire"] = 9000243952, 
				["Kamehameha Max"] = 9000245195, 
				Kamehameha = 8995538852, 
				Transform = 10446762289, 
				Jajanken = 8995545277, 
				["Instant Transmission"] = 8995547401, 
				["Explosive Wave"] = 8995549434, 
				["Senzu Bean"] = 8995553609, 
				["Destructo Disc"] = 8995557234, 
				["Solar Flare"] = 8995559419, 
				["Dragon Throw Attempt"] = 9000247100, 
				["Dragon Throw"] = 9000248965, 
				["Meteor Smash Attempt"] = 9000250472, 
				["Meteor Smash"] = 9000253195, 
				["Gut Punch"] = 9000272839, 
				Transcendence = 9000274037, 
				Barrage = 10455636567, 
				["Meteor Combination Attempt"] = 9083907352, 
				["Meteor Combination"] = 9083910504, 
				["Spirit Bomb Start"] = 9083935295, 
				["Spirit Bomb Loop"] = 9083929820, 
				["Spirit Bomb"] = 9083937924, 
				Godbind = 9083940979, 
				["Grudgeless Strike"] = 9083945838, 
				["Super God Fist"] = 9083952828, 
				["Super God Shock Flash"] = 9083956238, 
				["Celestial Whirlwind Pose"] = 9083969948, 
				["Celestial Whirlwind"] = 9083973324, 
				["Instinct Pose"] = 9083978473, 
				Instinct = 9083984834, 
				["Autonomous Fist"] = 9083993691, 
				["Unpolished Instinct"] = 9083996482
			}, 
			Movement = {
				Run = 10455589469, 
				Walk = 10455591976
			}, 
			Idle = {
				Idle = 10455579066
			}
		}, 
		zaihop = {
			Action = {
				["LMB-1"] = 7756678348, 
				["LMB-2"] = 7756680481, 
				["LMB-3"] = 7756686359, 
				["LMB-4"] = 7758466340, 
				["Home Run"] = 7759029193, 
				["Ban Hammer"] = 7764660173, 
				["Shovel Slam"] = 7764964415, 
				["Shovel Spin"] = 7767935194, 
				["Shovel Gun"] = 7769165261, 
				["Shovel Sinkhole"] = 7777096891, 
				["SS Startup"] = 7807883818, 
				["SS Leap"] = 7807889469, 
				["SS Spin Idle"] = 7807891660, 
				["SS Finish"] = 7807886164, 
				ForwardDash = 5601361906
			}, 
			Movement = {
				Run = 7756147590, 
				Walk = 7756149708
			}, 
			Idle = {
				Idle = 7756145559
			}
		}, 
		["Candy Cutlass"] = {
			Action = {
				["LMB-1"] = 8339433631, 
				["LMB-2"] = 8339494888, 
				["LMB-3"] = 8339540203, 
				["LMB-4"] = 8347065812, 
				["Sword Slashes"] = 8284745181, 
				["Second Degree Burn"] = 8285521172, 
				["Naughty List Attempt"] = 8287443015, 
				["Naughty List Hit"] = 8287444401, 
				["Naughty List Victim"] = 8287447145, 
				["Naughty List Victim Kick"] = 8294844534, 
				["Ice Stampede"] = 8294686957, 
				["Christmas Spirit"] = 8301744269, 
				["Candy Spit"] = 8444886216, 
				["Insulin Spike Jab"] = 8321963485, 
				["Insulin Spike Hit"] = 8335322126, 
				["Insulin Spike Victim"] = 8335332078, 
				["Insulin Spike Victim Knockback"] = 8335338603, 
				PoseTransition = 8420240312, 
				PoseIdle = 8420237840
			}, 
			Movement = {
				Run = 8368299567, 
				Walk = 8368306574
			}, 
			Idle = {
				Idle = 8368309134
			}
		}, 
		["Mero Mero"] = {
			Action = {
				["Eat Fruit"] = 8541951813, 
				["LMB-1"] = 8553461932, 
				["LMB-2"] = 8553466608, 
				["LMB-3"] = 8553469369, 
				["LMB-4"] = 8553476508, 
				["Hardening Sin Start"] = 8563711919, 
				["Hardening Sin Loop"] = 8563721544, 
				["Petrification Aroma"] = 10881095387, 
				["Grand Petrification Aroma"] = 8564731199, 
				["Pistol Kiss Aim"] = 8573835767, 
				["Pistol Kiss Shoot"] = 8573839521, 
				["Heartbreaker Use"] = 8602310890, 
				["Heartbreaker Hit"] = 8602313394, 
				["Heartbreaker Victim"] = 8602326715, 
				["Heartbreaker Victim KB"] = 8602328663, 
				["Easy Lover"] = 8614818815, 
				["Machine Gun Kiss"] = 8614831163, 
				PoseTransition = 10405294780, 
				PoseIdle = 10405298544
			}, 
			Idle = {
				Idle = 8531590159
			}
		}, 
		["Weather Report"] = {
			Action = {
				["LMB-1"] = 8990260713, 
				["LMB-2"] = 9481245541, 
				["LMB-3"] = 9481223928, 
				["LMB-4"] = 9481253071, 
				["Triple Air Cleave"] = 10203308028, 
				["Shock Barrage"] = 8941637069, 
				["Shock Barrage Finisher"] = 8941638648, 
				["Combustive Heatwave"] = 8963181689, 
				["Flare Ring"] = 10274186243, 
				["Lightning Strike Startup"] = 8990112524, 
				["Lightning Strike Hit"] = 8991485074, 
				["Lightning Strike Victim"] = 8991482812, 
				["Lightning Strike Camera"] = 8991499930, 
				["Devils Rainbow"] = 9492396219, 
				["Jet Airplane"] = 9492411353, 
				["Cloud Suit"] = 9492540658, 
				["Heavy Weather"] = 9492525212, 
				["Heavy Weather Clouds"] = 10368167035, 
				["Default Clouds"] = 10368210454, 
				["Thousand Volt Plexus"] = 10023924348, 
				["Ice Breath"] = 10274178015, 
				["Lung Exhaustion"] = 10046319500, 
				["Lung Victim"] = 10046328617, 
				["WOD Uncharged"] = 10062966645, 
				["WOD Startup"] = 10062947046, 
				["WOD Charging"] = 10062954336, 
				["WOD Finisher"] = 10064922298, 
				["Frog Transition"] = 6350085587, 
				["Counter Startup"] = 10129780091, 
				["Counter Loop"] = 10129784508, 
				["Oxidation Startup"] = 10158381439, 
				["Blood Oxidation"] = 10158384930, 
				["Oxidation Victim"] = 10158471514, 
				["Air Bomb"] = 10235539523, 
				["Air Bullets Startup"] = 10173994074, 
				["Air Bullets Loop"] = 10173996202, 
				PoseStart = 10367157472, 
				PoseLoop = 10367160860
			}, 
			Movement = {
				Run = 7037969480, 
				Walk = 6707573199, 
				SummonedRun = 7037969480, 
				SummonedWalk = 6707573199
			}, 
			Idle = {
				StandIdle = 8933510017, 
				Idle = 8933602062
			}
		}, 
		Guts = {
			Action = {
				["LMB-1"] = 10640223644, 
				["LMB-2"] = 10640224663, 
				["LMB-3"] = 10640225897, 
				["LMB-4"] = 10640227078, 
				["Blood & Guts"] = 10676333442, 
				["Loose Cannon"] = 10618519393
			}, 
			Movement = {
				Walk = 10640189679, 
				Run = 10640191645
			}, 
			Idle = {
				Idle = 10608986830
			}
		}, 
		["Weather Report Crawl"] = {
			Action = {
				CrawlTransition = 10010413439
			}, 
			Movement = {
				CrawlMovement = 10010423650
			}, 
			Idle = {
				CrawlIdle = 10010420896
			}
		}, 
		Brickbattle = {
			Action = {
				Sample = 1, 
				["Hammer Slam"] = 8987751217, 
				["Fire Rocket"] = 8987760061, 
				["Place Bomb"] = 8987763805, 
				["Build Wall"] = 8987767273, 
				["Item Pull"] = 9281773907, 
				["Equip Paint"] = 9281777834, 
				["Fire Paint"] = 9281780974, 
				["Slingshot Fling"] = 9489815142, 
				["Throw Superball"] = 9489777674, 
				["Monster Mash"] = 35654637, 
				["LMB-1"] = 9489835071, 
				["LMB-2"] = 9489848902, 
				["LMB-3"] = 9489855712, 
				["LMB-4"] = 9489863948
			}, 
			Movement = {
				Run = 180426354, 
				Walk = 180426354, 
				Jump = 8958971025, 
				Fall = 8958971025
			}, 
			Idle = {
				Idle = 180435571
			}
		}, 
		Banisher = {
			Action = {
				PoseIdle = 9882291671
			}, 
			Idle = {
				Idle = 9839675543
			}, 
			Movement = {
				Walk = 6877996750, 
				Run = 7037969480, 
				SummonedWalk = 6877996750
			}
		}, 
		["Stone Free"] = {
			Action = {
				["Ora Kicks"] = 9554010452, 
				Barrage = 6331004626, 
				["Spider Tack"] = 9554023294, 
				["Pitcher Fly Throw"] = 9554012774, 
				["Pitcher Fly Camera"] = 9554027739, 
				["Pitcher Fly Hit"] = 9554028664, 
				["Pitcher Fly Victim"] = 9554029803, 
				["Cuff Bash"] = 9574861170, 
				["Chin Crusher"] = 9575094870, 
				["Meteor Strike"] = 9605034134, 
				["Meteor Strike 2"] = 9605040105
			}, 
			Idle = {
				Idle = 10640153820, 
				StandIdle = 10640152257
			}, 
			Movement = {
				Walk = 10640156530, 
				SummonedRun = 9557545534, 
				SummonedWalk = 10640156530
			}
		}, 
		["Mortal Man"] = {
			Action = {}, 
			Idle = {
				Idle = 7294684954
			}
		}, 
		["Chrono Sentinel"] = {
			Action = {
				Grab = 11110729280, 
				Throw = 11110730939, 
				ThrowVictim = 11110732132
			}, 
			Movement = {
				Walk = 10660424510, 
				Run = 10982240350, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				Idle = 10660237915
			}
		}, 
		STWR_R = {
			Action = {
				["LMB-1"] = 10618698480, 
				["LMB-2"] = 10618701589, 
				["LMB-3"] = 10618705069, 
				["LMB-4"] = 10618709770, 
				StandBlock = 10808688837, 
				StandBlockHit1 = 10808692075, 
				StandBlockHit2 = 10808695355, 
				StandBlockHit3 = 10808697696, 
				StandBlockBreak = 10808701329, 
				BarrageStartup = 10838298509, 
				Barrage = 10838301380, 
				BarrageFinisher = 10603516376, 
				BarrageClashEnd = 10839831781, 
				Grab = 10906128504, 
				Throw = 10906131878, 
				ThrowVictim = 10906132668
			}, 
			Movement = {
				Walk = 10856503017, 
				Run = 10856500879, 
				SummonedWalk = 10856503017, 
				SummonedRun = 10856500879, 
				ForwardDash = 10838677738, 
				BackwardDash = 10838687030, 
				LeftDash = 10838688196, 
				RightDash = 10838689289
			}, 
			Idle = {
				StandIdle = 11001154516, 
				Idle = 11001148965
			}
		}
	}
};
local l__anims__1 = v6.anims;
local function v7(p1)
	for v8, v9 in pairs((require(p1))) do
		l__anims__1[v8] = v9;
	end;
end;
local v10, v11, v12 = ipairs(script:GetChildren());
while true do
	v10(v11, v12);
	if not v10 then
		break;
	end;
	v12 = v10;
	local v13, v14 = pcall(v7, v11);
	if not v13 then
		warn(v14, v11);
	end;
end;
v6.anims.Urzan = v6.anims.Reaper;
v6.anims.Thug = v6.anims.Standless;
v6.anims["Futuristic Queen"] = v6.anims["Killer Queen"];
v6.anims.KCR = v6.anims["King Crimson"];
v6.anims["Party Starter"] = v6.anims["The World: Over Heaven"];
v6.anims.Cypher = v6.anims["The World: Over Heaven"];
v6.anims.ShadowLegs = v6.anims.ShadowDio;
v6.anims.StarPlatinumOVA = v6.anims["Star Platinum"];
v6.anims.Noob = v6.anims["The World: Over Heaven"];
v6.anims.DJNoob = v6.anims["The World: Over Heaven"];
v6.anims.HSTWR = v6.anims.STWR;
v6.anims.DTWHV = v6.anims.TWHV;
v6.anims["Boa H"] = v6.anims["Mero Mero"];
v6.anims.Dio = v6.anims["The World"];
v6.anims.Diavolo = v6.anims["King Crimson"];
v6.anims.Johnny = v6.anims.Tusk;
v6.anims["Gold Experience (Requiem)"] = v6.anims["Gold Experience"];
local v15, v16, v17 = pairs(v6.anims);
while true do
	local v18, v19 = v15(v16, v17);
	if not v18 then
		break;
	end;
	local v20 = {
		ForwardDash = 10451361960, 
		BackwardDash = 10451359576, 
		LeftDash = 10451363828, 
		RightDash = 10451365211
	};
	if not v19.Movement then
		v19.Movement = v2.Copy(v20);
	else
		v19.Movement = v2.Reconcile(v19.Movement, v20);
	end;
	if v19.Action then
		if not v19.Action.Block then
			v19.Action.Block = 7037951229;
		end;
		if not v19.Action.ComboBreaker then
			v19.Action.ComboBreaker = 9967760592;
		end;
		if not v19.Action.DeathAnim then
			v19.Action.DeathAnim = 7070248368;
		end;
	end;
end;
local u2 = Instance.new("Animation");
local v21 = require(game.ReplicatedStorage.ReplicatedModules.Stands);
local v22 = game:GetService("RunService"):IsStudio();
for v23, v24 in pairs(require(game.ReplicatedStorage.ReplicatedModules.Skins).Funcs.GetSkins()) do
	local v25 = v21[tonumber(v23)];
	for v26, v27 in pairs(v24) do
		if l__anims__1[v27] and l__anims__1[v27] ~= l__anims__1[v25] then
			l__anims__1[v27] = v2.Reconcile(l__anims__1[v27], (v2.Copy(l__anims__1[v25], true)));
			if v22 then

			end;
		else
			l__anims__1[v27] = l__anims__1[v25];
			if v22 then

			end;
		end;
	end;
end;
function v6.SearchAnim(p2, p3)
	if not v6.anims[p2] then
		return;
	end;
	for v28, v29 in pairs(v6.anims[p2]) do
		for v30, v31 in pairs(v29) do
			if v30 == p3 then
				return v31, v28;
			end;
		end;
	end;
end;
function v6.GetAnim(p4, p5)
	local v32 = nil;
	local v33 = nil;
	v33, v32 = v6.SearchAnim(p4, p5);
	if not v33 or not v32 then
		return;
	end;
	return {
		Animation = v33, 
		Priority = v32
	};
end;
function v6.GetAnims(p6)
	if not v6.anims[p6] then
		return;
	end;
	local v34 = {};
	for v35, v36 in pairs(v6.anims[p6]) do
		for v37, v38 in pairs(v36) do
			v34[v37] = {
				Animation = v38, 
				Priority = v35
			};
		end;
	end;
	return v34;
end;
(function(p7)
	local v39 = {};
	for v40, v41 in pairs(p7) do
		for v42, v43 in pairs(v41) do
			for v44, v45 in pairs(v43) do
				if type(v45) ~= "table" and type(v45) ~= "userdata" then
					local v46 = "rbxassetid://" .. v45;
					if v39[v46] then
						p7[v40][v42][v44] = v39[v46];
					else
						local v47 = u2:Clone();
						v47.Name = v44;
						v47.AnimationId = v46;
						v39[v46] = v47;
						p7[v40][v42][v44] = v47;
					end;
				end;
			end;
		end;
	end;
end)(v6.anims);
local u3 = {};
function v6.loadAnims(p8, p9)
	local l__Parent__48 = p9.Parent;
	u3[l__Parent__48] = {};
	u3[l__Parent__48][p8] = {};
	if not v6.anims[p8] or not p9:IsDescendantOf(workspace) then
		warn(p8, "not found in anims table");
		return;
	end;
	for v49, v50 in pairs(v6.anims[p8]) do
		for v51, v52 in pairs(v50) do
			local v53 = p9:LoadAnimation(v52);
			v53.Priority = Enum.AnimationPriority[v49];
			u3[l__Parent__48][p8][v51] = v53;
		end;
	end;
end;
local u4 = { "ForwardDash", "BackwardDash", "LeftDash", "RightDash" };
function v6.playClient(p10, p11, p12, p13, p14, p15)
	if not p10 then
		return;
	end;
	if p14 then
		local v54 = p14.Parent or (p14:FindFirstAncestorOfClass("Model") or (game:GetService("Players").LocalPlayer.Character or nil));
	else
		v54 = game:GetService("Players").LocalPlayer.Character or nil;
	end;
	local v55 = nil;
	local v56 = false;
	local v57 = nil;
	if p15 then
		if v54 and v54:FindFirstChild("Data") and v54.Data:FindFirstChild("Skin") then
			v57 = v54.Data.Skin:GetAttribute("SkinName");
		end;
	else
		local v58 = game:GetService("Players"):GetPlayerFromCharacter(v54);
		if v58 then
			v57 = v58.Data.Skin:GetAttribute("SkinName");
			if v58.Character then
				local l__Stand__59 = v58.Character:FindFirstChild("Stand");
				if l__Stand__59 and l__Stand__59:GetAttribute("SkinName") then
					v57 = l__Stand__59:GetAttribute("SkinName");
				end;
			end;
		end;
	end;
	if not u3[v54] then
		u3[v54] = {};
	end;
	if not v57 then
		if not u3[v54][p10] then
			u3[v54][p10] = {};
		end;
		if u3[v54][p10][p11] then
			v55 = u3[v54][p10][p11];
			v56 = true;
		end;
	else
		if not u3[v54][v57] then
			u3[v54][v57] = {};
		end;
		if u3[v54][v57][p11] then
			v55 = u3[v54][v57][p11];
			v56 = true;
		end;
	end;
	if not v56 then
		local v60 = p14 or (v54.Humanoid or nil);
		if not v60 then
			if v22 then
				warn("No Animation Humanoid found");
			end;
			return;
		end;
		if not v60:IsDescendantOf(workspace) then
			warn("humanoid not descendant of workspace");
			return;
		end;
		local v61 = nil;
		local v62 = nil;
		if v57 then
			local v63, v64 = v6.SearchAnim(v57, p11);
			v61 = v63;
			v62 = v64;
		end;
		if not v61 and not v62 then
			local v65, v66 = v6.SearchAnim(p10, p11);
			v61 = v65;
			v62 = v66;
		end;
		if not p12 then
			p12 = v62;
		end;
		if v61 then
			local v67 = v60:LoadAnimation(v61);
			if v57 then
				u3[v54][v57][p11] = v67;
			else
				u3[v54][p10][p11] = v67;
			end;
			if p12 then
				v55.Priority = p12;
			end;
			v56 = true;
		end;
	end;
	if not v55 or not v56 then
		return;
	end;
	if table.find(u4, p11) then
		v54:SetAttribute("Dashing", true);
	end;
	local u5 = v3.new();
	u5:Add(v55.Stopped:Connect(function()
		if table.find(u4, p11) then
			v54:SetAttribute("Dashing", false);
		end;
		if u3[v54][p10] then
			u3[v54][p10][p11] = nil;
		end;
		u5:Destroy();
	end));
	v55:Play(nil, nil, p13 and 1);
	return v55;
end;
function v6.adjustAnimSpeed(p16, p17, p18, p19)
	local v68 = p19 and p19.Parent or game.Players.LocalPlayer.Character;
	local v69 = nil;
	local v70 = false;
	local v71 = nil;
	local v72 = game:GetService("Players"):GetPlayerFromCharacter(v68);
	if v72 then
		v71 = v72.Data.Skin:GetAttribute("SkinName");
		if v72.Character then
			local l__Stand__73 = v72.Character:FindFirstChild("Stand");
			if l__Stand__73 and l__Stand__73:GetAttribute("SkinName") then
				v71 = l__Stand__73:GetAttribute("SkinName");
			end;
		end;
	end;
	if v71 and u3[v68] and u3[v68][v71] and u3[v68][v71][p17] then
		v69 = u3[v68][v71][p17];
		v70 = true;
	end;
	if not v70 and u3[v68] and u3[v68][p16] and u3[v68][p16][p17] then
		v69 = u3[v68][p16][p17];
	end;
	v69:AdjustSpeed(p18 and 1);
	return v69;
end;
function v6.stopClient(p20, p21, p22, p23)
	local v74 = p22 or (game.Players.LocalPlayer.Character or game.Players.LocalPlayer.CharacterAdded:Wait());
	local v75 = nil;
	if not p23 then
		local v76 = game:GetService("Players"):GetPlayerFromCharacter(v74);
		if v76 then
			v75 = v76.Data.Skin:GetAttribute("SkinName");
			if v76.Character then
				local l__Stand__77 = v76.Character:FindFirstChild("Stand");
				if l__Stand__77 and l__Stand__77:GetAttribute("SkinName") then
					v75 = l__Stand__77:GetAttribute("SkinName");
				end;
			end;
		end;
	end;
	local v78 = nil;
	if v75 then
		v78 = u3[v74] and (u3[v74][v75] and u3[v74][v75][p21]);
	end;
	if not v78 then
		v78 = u3[v74] and (u3[v74][p20] and u3[v74][p20][p21]);
	end;
	if v78 then
		if v78.IsPlaying then
			v78:Stop();
			return;
		else
			return;
		end;
	elseif not p23 then
		if v22 then
			warn(p20, p21, debug.traceback("anim not found for stand"));
		end;
		return;
	end;
	local v79, v80, v81 = ipairs(v74:FindFirstChildWhichIsA("Humanoid"):GetPlayingAnimationTracks());
	while true do
		v79(v80, v81);
		if not v79 then
			break;
		end;
		v81 = v79;
		if v80.Name == p20 .. "-" .. p21 then
			v80:Stop();
		end;	
	end;
end;
function v6.FindAnim(p24, p25, p26, p27)
	if p26 then
		local v82 = p26.Parent or (p26:FindFirstAncestorOfClass("Model") or (game:GetService("Players").LocalPlayer.Character or nil));
	else
		v82 = game:GetService("Players").LocalPlayer.Character or nil;
	end;
	local v83 = nil;
	if p27 then
		if v82 and v82:FindFirstChild("Data") and v82.Data:FindFirstChild("Skin") then
			v83 = v82.Data.Skin:GetAttribute("SkinName");
		end;
	else
		local v84 = game:GetService("Players"):GetPlayerFromCharacter(v82);
		if v84 then
			v83 = v84.Data.Skin:GetAttribute("SkinName");
			if v84.Character then
				local l__Stand__85 = v84.Character:FindFirstChild("Stand");
				if l__Stand__85 and l__Stand__85:GetAttribute("SkinName") then
					v83 = l__Stand__85:GetAttribute("SkinName");
				end;
			end;
		end;
	end;
	local v86 = nil;
	local v87 = nil;
	if v83 then
		local v88, v89 = v6.SearchAnim(v83, p25);
		v86 = v88;
		v87 = v89;
	end;
	if not v86 and not v87 then
		local v90, v91 = v6.SearchAnim(p24, p25);
		v86 = v90;
		v87 = v91;
	end;
	return v86, v87;
end;
return v6;
