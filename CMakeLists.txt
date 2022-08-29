
project(ImGui)
cmake_minimum_required(VERSION 3.5)

include_directories(include)

file(GLOB ImGui_SRC
    "imconfig.h"
	"imgui.h"
	"imgui.cpp"
	"imgui_draw.cpp"
	"imgui_internal.h"
	"imgui_widgets.cpp"
	"imstb_rectpack.h"
	"imstb_textedit.h"
	"imstb_truetype.h"
	"imgui_demo.cpp"
    "imgui_tables.cpp"
)

add_library(imgui STATIC ${ImGui_SRC})

