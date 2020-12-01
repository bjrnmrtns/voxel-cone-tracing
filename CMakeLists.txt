project(voxel-cone-tracing)

find_package(GLEW REQUIRED)

add_executable(voxel-cone-tracing
voxel-cone-tracing.cpp
Source/Graphic/Texture3D.cpp
Source/Graphic/Texture2D.cpp
Source/Graphic/Graphics.cpp
Source/Graphic/FBO/FBO.cpp
Source/Graphic/Renderer/MeshRenderer.cpp
Source/Graphic/Camera/PerspectiveCamera.cpp
Source/Graphic/Camera/Camera.cpp
Source/Graphic/Camera/OrthographicCamera.cpp
Source/Graphic/Material/Shader.cpp
Source/Graphic/Material/Material.cpp
Source/Graphic/Material/MaterialStore.cpp
Source/Utility/External/tiny_obj_loader.cpp
Source/Utility/ObjLoader.cpp
Source/Application.cpp
Source/Scene/Scenes/CornellScene.cpp
Source/Scene/Scenes/GlassScene.cpp
Source/Scene/Scenes/DragonScene.cpp
Source/Scene/Scenes/MultipleObjectsScene.cpp
Source/Shape/StandardShapes.cpp
Source/Shape/Mesh.cpp
Source/Shape/Transform.cpp
Source/Time/Time.cpp
)


target_link_libraries(voxel-cone-tracing PRIVATE
        GL
		GLEW
        SOIL
        glfw
)
