cmake_minimum_required (VERSION 2.8)
project (TRON_ServerRes)
add_library (TRON_ServerRes SHARED 
	MAIN.CPP
	ServerRes.rc)
set_target_properties(TRON_ServerRes 
	PROPERTIES OUTPUT_NAME SRes)
