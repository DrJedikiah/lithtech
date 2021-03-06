cmake_minimum_required (VERSION 2.8)
project (ClientShellDLL)

add_subdirectory(../../Engine/libs/MFCStub ${CMAKE_CURRENT_BINARY_DIR}/MFCStub)
add_subdirectory(../../Engine/libs/stdlith ${CMAKE_CURRENT_BINARY_DIR}/stdlith)
add_subdirectory(../../Engine/libs/ButeMgr ${CMAKE_CURRENT_BINARY_DIR}/ButeMgr)
add_subdirectory(../../Engine/libs/CryptMgr ${CMAKE_CURRENT_BINARY_DIR}/CryptMgr)
add_subdirectory(../../Engine/libs/lith ${CMAKE_CURRENT_BINARY_DIR}/lith)
add_subdirectory(../../Engine/libs/RegMgr ${CMAKE_CURRENT_BINARY_DIR}/RegMgr)
add_subdirectory(../../NOLF2/Libs/LTGUIMgr ${CMAKE_CURRENT_BINARY_DIR}/LTGUIMgr)
#add_subdirectory(../Libs/ServerDir ${CMAKE_CURRENT_BINARY_DIR}/ServerDir)

add_library (ClientShellDLL SHARED
	AccuracyMgr.cpp
	AccuracyVisualization.cpp
	ActivateObjectFX.cpp
	AimMagnetFX.cpp
	AimMgr.cpp
	AutoTargetMgr.cpp
	BaseMenu.cpp
	BaseScreen.cpp
	BindMgr.cpp
	CameraOffsetMgr.cpp
	CharacterDisplay.cpp
	CharacterFX.cpp
	CheatMgr.cpp
	client_physics.cpp
	ClientConnectionMgr.cpp
	ClientDB.cpp
	ClientFXInstance.cpp
	ClientFXMgr.cpp
	ClientFXSequence.cpp
	ClientInfoMgr.cpp
	ClientMeleeCollisionController.cpp
	ClientNodeTrackerContext.cpp
	ClientPhysicsCollisionMgr.cpp
	ClientSaveLoadMgr.cpp
	ClientSoundMgr.cpp
	ClientSoundMixer.cpp
	ClientSoundNonPointFX.cpp
	ClientUtilities.cpp
	ClientVoteMgr.cpp
	ClientWeapon.cpp
	ClientWeaponMgr.cpp
	ClientWeaponUtils.cpp
	CMoveMgr.cpp
	ConditionalAnimationController.cpp
	ControlPointSFX.cpp
	Credits.cpp
	CTFFlagBaseSFX.cpp
	CTFFlagSFX.cpp
	CursorMgr.cpp
	CustomCtrls.cpp
	DamageFXMgr.cpp
	DebugLineFX.cpp
	DynamicSectorVolumeFX.cpp
	EntryToolLockFX.cpp
	ExplosionFX.cpp
	FinishingMoveFX.cpp
	FlashLight.cpp
	../Shared/ForceVolume.cpp
	ForensicObjectFX.cpp
	FrameStatConsoleInfo.cpp
	FullScreenTint.cpp
	GameClientShell.cpp
	GameRuleCtrls.cpp
	GameSettings.cpp
	GameStreamingMgr.cpp
	GlobalClientMgr.cpp
	GlobalsInit.cpp
	HeadBobMgr.cpp
	HitBox.cpp
	../Shared/HostOptionsMapMgr.cpp
	HUDActivate.cpp
	HUDActivateObject.cpp
	HUDAmmo.cpp
	HUDAmmoStack.cpp
	HUDAnimation.cpp
	HUDArmor.cpp
	HUDBar.cpp
	HUDBuildVersion.cpp
	HUDChatInput.cpp
	HUDControlPoint.cpp
	HUDControlPointBar.cpp
	HUDCrosshair.cpp
	HUDCTFBase.cpp
	HUDCTFFlag.cpp
	HUDDamageDir.cpp
	HUDDebug.cpp
	HUDDebugInput.cpp
	HUDDecision.cpp
	HUDDialogue.cpp
	HUDDistance.cpp
	HUDEndRoundMessage.cpp
	HUDEvidence.cpp
	HUDFlashlight.cpp
	HUDFocus.cpp
	HUDGear.cpp
	HUDGearList.cpp
	HUDGrenade.cpp
	HUDHealth.cpp
	HUDHealth2.cpp
	HUDInstinct.cpp
	HUDInventory.cpp
	HUDInventoryList.cpp
	HUDItem.cpp
	HUDMessage.cpp
	HUDMessageQueue.cpp
	HUDMeter.cpp
	HUDMgr.cpp
	HUDNavMarker.cpp
	HUDNavMarkerMgr.cpp
	HUDOverlay.cpp
	HUDPaused.cpp
	HUDPlayerList.cpp
	HUDRadio.cpp
	HUDRespawn.cpp
	HUDScoreDiff.cpp
	HUDScores.cpp
	HUDSlowMo.cpp
	HUDSonicBreath.cpp
	HUDSpectator.cpp
	HUDSprintBoost.cpp
	HUDSubtitles.cpp
	HUDSwap.cpp
	HUDTeamScores.cpp
	HUDTimer.cpp
	HUDTitleSafeAreaNTSC.cpp
	HUDToolSelect.cpp
	HUDTransmission.cpp
	HUDVote.cpp
	HUDWeapon.cpp
	HUDWeaponBreak.cpp
	HUDWeaponList.cpp
	InterfaceMgr.cpp
	InterfaceResMgr.cpp
	JumpVolumeFX.cpp
	LadderFX.cpp
	LadderMgr.cpp
	LayoutDB.cpp
	LeanMgr.cpp
	LightScaleMgr.cpp
	LoadingScreen.cpp
	LoadingScreenLayout.cpp
	MarkSFX.cpp
	MenuEndRound.cpp
	MenuMgr.cpp
	MenuMission.cpp
	MenuSystem.cpp
	MessageBox.cpp
	MissionMgr.cpp
	ModelDecalMgr.cpp
	NavMarkerFX.cpp
	NodeBlink.cpp
	NodeController.cpp
	objectdetector.cpp
	OrbitalScreenshotMgr.cpp
	PerformanceLog.cpp
	PerformanceLogMgr.cpp
	PerformanceMgr.cpp
	../../Engine/sdk/inc/performancemonitorhook.cpp
	PerformanceTest.cpp
	PhysicsCollisionSystemFX.cpp
	PhysicsConstraintFX.cpp
	PickupItemFX.cpp
	PlayerBodyMgr.cpp
	PlayerCamera.cpp
	PlayerLureFX.cpp
	PlayerMgr.cpp
	PlayerSoundFX.cpp
	PlayerStats.cpp
	PlayerViewAttachmentMgr.cpp
	PolyGridFX.cpp
	ProfileMgr.cpp
	ProjectileFX.cpp
	RenderTargetFX.cpp
	RenderTargetGroupFX.cpp
	ScatterFX.cpp
	ScmdConsoleDriver_CShell.cpp
	ScoresCtrl.cpp
	ScreenAudio.cpp
	ScreenConfigure.cpp
	ScreenControls.cpp
	ScreenCrosshair.cpp
	ScreenDisplay.cpp
	ScreenEffectFX.cpp
	ScreenFailure.cpp
	ScreenGame.cpp
	ScreenHostDownload.cpp
	ScreenHostVoting.cpp
	ScreenHostWeapons.cpp
	ScreenJoystick.cpp
	ScreenLoad.cpp
	ScreenMain.cpp
	ScreenMgr.cpp
	ScreenMouse.cpp
	ScreenMutePlayer.cpp
	ScreenOptions.cpp
	ScreenPerformance.cpp
	ScreenPerformanceAdvanced.cpp
	ScreenPerformanceCPU.cpp
	ScreenPerformanceGPU.cpp
	ScreenPlayer.cpp
	ScreenPlayerLoadout.cpp
	ScreenPlayerTeam.cpp
	ScreenPostload.cpp
	ScreenPreload.cpp
	ScreenProfile.cpp
	ScreenSave.cpp
	ScreenSingle.cpp
	ScreenTeam.cpp
	ScreenTintMgr.cpp
	ScreenVote.cpp
	ScreenWeapons.cpp
	SearchLightFX.cpp
	SFXMgr.cpp
	ShatterEffect.cpp
	ShatterEffectMgr.cpp
	ShellCasingFX.cpp
	SnowFX.cpp
	SpecialFXList.cpp
	SpecialFXNotifyMessageHandler.cpp
	SpecialMoveFX.cpp
	SpecialMoveMgr.cpp
	Stdafx.cpp
	TargetMgr.cpp
	TeamClientFXSFX.cpp
	TriggerFX.cpp
	TurretFX.cpp
	UserNotificationMgr.cpp
	UserNotifiers.cpp
	VehicleMgr.cpp
	VKDefs.cpp
	VolumetricLightFX.cpp
	WeaponDisplay.cpp
	WeaponFX.cpp
	Game_ClientShell.rc
	#Win32
	ScreenHost.cpp
	ScreenHostLevels.cpp
	ScreenHostOptionFile.cpp
	ScreenHostOptions.cpp
	ScreenMulti.cpp
	ServerBrowserCtrl.cpp)
set_target_properties(ClientShellDLL 
	PROPERTIES OUTPUT_NAME CShell)
add_definitions (-D_CRT_SECURE_NO_WARNINGS -D_CLIENTBUILD -DMEMTRACK_CLIENT)
include_directories (../Shared 
	../../Engine/sdk/inc
	../../Engine/libs/MFCStub
	../../Engine/libs/stdlith
	../../Engine/libs/ButeMgr
	../../Engine/libs/CryptMgr
	../../Engine/libs/lith
	../../Engine/libs/RegMgr
	../../NOLF2/Libs/LTGUIMgr
	#../Libs/ServerDir
	../ClientRes)
target_link_libraries(ClientShellDLL
	MFCStub
	Lib_StdLith
	ButeMgr
	CryptMgr
	Lib_Lith
	RegMgr
	LTGUIMgr
	#ServerDir
	winmm.lib)