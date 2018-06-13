#Indirect-Rendering-With-Compute-Shaders

An example of drawing numerous instances in Unity3D using Graphics.DrawMeshInstancedIndirect.

##Features

- Use compute buffers and compute shaders
- Draw things using Graphics.DrawMeshInstancedIndirect
- Frustum culling in a compute shader
- Occlusion culling with HierarchicalZBuffer in a compute shader
- Extending camera frustum towards light to include shadow casting objects
- LOD objects by distance in a compute shader


##TODO
- Implement Kostas approach:
	- Dispatch the compute shader only once for all instances
	- Implement Stream-Compaction
	- Batch LOD meshes in to large buffers
- Try out Raster Occlusion instead of Hi-Z (See "NVidia Siggraph 2014" & "Github - nvpro-samples" below)

##Useful links

[Sakib Saikia - Going Indirect on UE3](https://sakibsaikia.github.io/graphics/2017/08/18/Going-Indirect-On-UE3.html)

[Kostas Anagnostou - GPU Driven Rendering Experiments](http://bit.ly/Kostas-GPUDrivenRenderingExperiments)

[Kostas Anagnostou - Experiments in GPU-based occlusion culling](https://interplayoflight.wordpress.com/2017/11/15/experiments-in-gpu-based-occlusion-culling/)

[Kostas Anagnostou - Experiments in GPU-based occlusion culling part 2](https://interplayoflight.wordpress.com/2018/01/15/experiments-in-gpu-based-occlusion-culling-part-2-multidrawindirect-and-mesh-lodding/)

[RasterGrid - Hierarchical-Z map based occlusion culling](http://rastergrid.com/blog/2010/10/hierarchical-z-map-based-occlusion-culling/)

[StackOverflow - Hierachical Z-Buffering for occlusion culling](https://gamedev.stackexchange.com/questions/112155/hierachical-z-buffering-for-occlusion-culling)

[bazhenovc -  GPU Driven Occlusion Culling in Life is Feudal ](https://bazhenovc.github.io/blog/post/gpu-driven-occlusion-culling-slides-lif/)

[NVIDIA - Siggraph 2014 - Scene Rendering Techniques](http://on-demand.gputechconf.com/siggraph/2014/presentation/SG4117-OpenGL-Scene-Rendering-Techniques.pdf)

[Github - nvpro-samples/gl_occlusion_culling](https://github.com/nvpro-samples/gl_occlusion_culling)

[GPU Gems 2 - Hardware Occlusion Queries Made Useful](https://developer.nvidia.com/gpugems/GPUGems2/gpugems2_chapter06.html)

[ARM Developer Center - hiz_cull.cs](https://arm-software.github.io/opengl-es-sdk-for-android/hiz__cull_8cs_source.html)

[L. Spiro - Tightly Culling Shadow Casters for Directional Lights (Part 1)](http://lspiroengine.com/?p=153)

[L. Spiro - Tightly Culling Shadow Casters for Directional Lights (Part 2)](http://lspiroengine.com/?p=187)

[nonoptimalrobot - Shadow Volume Culling](https://nonoptimalrobot.wordpress.com/2012/04/19/shadow-volume-culling/)