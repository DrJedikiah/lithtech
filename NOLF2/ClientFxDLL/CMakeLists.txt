# FIXME: Looks like the code in Engine/clientfx is newer
project(NOLF2_ClientFXDLL)

add_library(${PROJECT_NAME} SHARED
	BaseFx.cpp
	bouncychunkfx.cpp
	camjitterfx.cpp
	camwobblefx.cpp
	clientfx.cpp
	CreateFX.cpp
	cycletimer.cpp
	../Shared/DebugNew.cpp
	dynalightfx.cpp
	fallingstufffx.cpp
	FlareSpriteFX.cpp
	lightningfx.cpp
	LTBbouncychunkfx.cpp
	ltbmodelfx.cpp
	../../sdk/inc/ltmodule.cpp
	../../sdk/inc/ltquatbase.cpp
	nullfx.cpp
	ParticleSystemFX.cpp
	playrandomsoundfx.cpp
	playsoundfx.cpp
	polyfanfx.cpp
	polytubefx.cpp
	spritefx.cpp
	spritesystemfx.cpp
	stdafx.cpp)

set_target_properties(${PROJECT_NAME}
	PROPERTIES OUTPUT_NAME ClientFx
	SUFFIX .fxd)

add_definitions(-DNOPS2 -DMEMTRACK_CLIENTFX)

include_directories(../Shared
	../../sdk/inc
	../../libs/MFCStub
	../../libs/stdlith)

if(CMAKE_COMPILER_IS_GNUCXX)
	set_target_properties(${PROJECT_NAME} PROPERTIES COMPILE_FLAGS "-fpermissive")
endif(CMAKE_COMPILER_IS_GNUCXX)
