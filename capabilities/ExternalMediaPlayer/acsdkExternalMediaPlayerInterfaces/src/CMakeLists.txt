include(${AVS_CORE}/build/BuildDefaults.cmake)

add_library(acsdkExternalMediaPlayerInterfaces SHARED
    AdapterUtils.cpp)

target_include_directories(acsdkExternalMediaPlayerInterfaces PUBLIC
    "${acsdkExternalMediaPlayerInterfaces_SOURCE_DIR}/include"
)

target_link_libraries(acsdkExternalMediaPlayerInterfaces
    AVSCommon)

# install target
asdk_install()
