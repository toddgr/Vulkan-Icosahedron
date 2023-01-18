# Vulkan-Playground
 Experimentation with Vulkan CS 559: Vulkan class at Oregon State University!
 
 Main branch is source code provided by Dr. Bailey.
 
Mike Bailey, Oregon State University
mjb@cs.oregonstate.edu

The class notes for which this program was written can be found here:
http://cs.oregonstate.edu/~mjb/vulkan

## Keyboard commands:
* `'i', 'I'`: Toggle using a vertex buffer only vs. a vertex/index buffer
* `'l', 'L'`: Toggle lighting off and on
* `'m', 'M'`: Toggle display mode (textures vs. colors, for now)
* `'p', 'P'`: Pause the animation
* `'q', 'Q'`: Esc: exit the program
* `'r', 'R'`: Toggle rotation-animation and using the mouse

This code occassionally uses #defines for environment-specific-isms:

`_WIN32`		Windows

`__linux__`    Linux

`__GNUC__`	GNU compiler


There are some pieces of the program that were tossed in to show how to do some things
they are not necessary in the program
#define them to turn them on, #undef them to turn them off
#undef EXAMPLE_OF_USING_DYNAMIC_STATE_VARIABLES

```There are also some spots where options are listed just to show you what could have happened here:
VkPipelineStageFlags waitAtBottom = VK_PIPELINE_STAGE_BOTTOM_OF_PIPE_BIT;
#ifdef CHOICES
VK_PIPELINE_STAGE_TOP_OF_PIPE_BIT = 0x00000001,
VK_PIPELINE_STAGE_DRAW_INDIRECT_BIT = 0x00000002,
. . .
#endif
```

## Create Your Own Vertex Data

This branch is used to get familiar with creating unique vertex data with Vulkan. 

The video demonstrating this vertex data can be found here:
