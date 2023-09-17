Stuff I've worked on.

### Knowledge Graph, Reliability Engineering (2016-Current)
![fubo-ws](https://github.com/halfvector/halfvector/assets/1817604/7f09870f-3255-465a-928d-e291c6b9a62c)

Job: Series B startup, scaleup, through IPO. The other seasons of Silicon Valley.

<br /><br />

### Augmented Reality Apps and Wearable Device Management (2014-2016)
![wearables](https://github.com/halfvector/halfvector/assets/1817604/e679000d-998a-4ecc-83ad-4f86a218662e)

Job: Wild seed stage startup, basically Season 1 of Silicon Valley.

<br /><br />
  
### Multi-layer materials (PBR/BRDFs) (2013)
![brdf-2](https://github.com/halfvector/halfvector/assets/1817604/c83a4d95-cf74-44d3-9e76-718370d157c6)

> Above, left to right: polished metal, rough metal, polished transparent acrylic over plastic, rough transparent acrylic over plastic.

![brdf-1](https://github.com/halfvector/halfvector/assets/1817604/e9aee861-c065-4370-aa91-a272d3b95425)

> Above, left to right: semitransparent smooth reflective acrylic over: smooth gold, rough gold, and a weird deeply absorbing plastic.

Physically-based deferred shading pipeline with various bidirectional reflectance distribution functions. Based heavily on work by folks like Oskar, Weidlich, and Wilkie.  
Combining aspects of Cook-Torrance, KSK, TriAce's BRDFs and various distributions (Gaussian, Phong, TrGgx/SmithG1, Beckmann).  

Plastics, glass, and metals could be rendered with the same shader code path by adjusting parameters for each layer and it's BRDF: roughness, complex IOR for metals and simple IOR for dielectrics, diffuse reflectance, and layer thickness.  

Screenshots are of a microfaceted KSK (Tr/GGX distributions) for specular and Oren Nayar for diffuse BRDF. Two layers attempting to simulate absorption and transmission, and focuses on physically based roughness using preconvoluted phong env maps.  

<br /><br />
    
### SOTA 3D Renderering & Shaders (2012)
![ScreenShot4573-pure-IBL-based-indirect-lighting](https://github.com/halfvector/halfvector/assets/1817604/85597c3a-1249-4575-8f9f-08cf94233d8c)
![ScreenShot4858-layered-brdfs-1024x484](https://github.com/halfvector/halfvector/assets/1817604/d8393d31-c442-4668-9c95-b43c24458e5e)


After a GDC 2012 conference where Tri-Ace demoed their ground-breaking Physically Based Rendering paper, I spent all my free time implementing every related paper for a year.  
IBL ambient lighting, complex reflectance for metals using roughness and biased mipmaps on prefiltered radiance environment maps.  
Every type of SSAO/bent-normals/contact-shadows related algorithms. And obviously of course lots of bloom.  

<br /><br />
  
### On-Air Social Media for MSNBC (2012)
![msnbc-social](https://github.com/halfvector/halfvector/assets/1817604/b7b59fdc-6556-4dc7-8578-393018bbd9d3)

Integrated Twitter and Facebook conversations with a third-party sentiment analysis engine and MSNBC's live TV show production.  
First premiered on "NOW with Alex Wagner".  
Mixture of Microsoft-stack, Linux rendering machines.  
My first "push to prod with 400k users".  

<br /><br />
  
### Surface Reader for New York Times (2011)
![nyt-table-custom](https://github.com/halfvector/halfvector/assets/1817604/8f13976a-43d0-4109-82b2-e13a575e7513)

C#  
Multi-finger and multi-person touch-based UI from scratch.  
Microsoft Surface Table. Silky smooth interactions.  

<br /><br />

### Game of Go for Microsoft (2011)
![game-of-go](https://github.com/halfvector/halfvector/assets/1817604/a5989c70-4737-4faa-94ff-f20e74bd9d5d)

C#  
Built from scratch for the Microsoft Surface.  
Leveraged Microsoft's High Performance Cluster connectivity to seriously challenge the player.  
One of my favorite contributions was thread-safety, deadlock-detection, and automatic event-marshalling that guaranteed callbacks ended up in the proper UI thread. This eventually became it's own library and was used for other projects.  
Sat in the lobby of one of the Microsoft campus buildings.  

<br /><br />

### Completely touch-based Concept Car for Chrysler (2009)
![chrysler-200c-interior](https://github.com/halfvector/halfvector/assets/1817604/f3c50467-bae0-49e1-8aa8-45f9ad14fb2f)

Built a gesture detector for the first ever touch film on the car interior that replaced all the buttons. It was immediately obvious that cars should not use touch panels until there's physical feedback.  
Interfaced with a cutting edge capacitive grid touch film via RS232.  
Coordinate dewarping, gesture recognition from noisy input.  
Web-service to support in-car communication for the demo between an iPhone app, Windows tablet, and car's hardware (HVAC, playing music, rolling down windows, starting the car).  

![detroit-autoshow](https://github.com/halfvector/halfvector/assets/1817604/d0dcb385-5acd-4e7c-8142-9927bd884a67)

<br /><br />

### Robotics Programming (2008)
![motion-module-on-rp-against-simulator-with-usar](https://github.com/halfvector/halfvector/assets/1817604/04ce245d-d82d-403c-936a-7b431351582a)
> The lengths I'll go to for Engineering Productivity

C++, Perl  
* 3D debug UI for observability of robotics planning and execution.  
* Sony Aibo simulator that runs real robotics code in an emulated environment to speed up iteration speed of locomotion code testing.  

My robotics code test environment using the hardware-accelerated physics engine PhysX (later acquired by NVidia).  
Another test environment was an Unreal Tournament 2004 mod.  
Intercepted and simulated PID joints accurately enough to even simulate an existing drift in our locomotion code that we saw on the physical field.  

![728886685_18e51a13e9_o](https://github.com/halfvector/halfvector/assets/1817604/75e8bb7e-34be-48ab-b02e-fc9de2403474)
> Above: My college sports team in the Robocup League.


<br /><br />

### Nintendo Emulator (2007)

![megaman-rom-proper-disassembly-clipped](https://github.com/halfvector/halfvector/assets/1817604/7084862f-81f8-4f45-803e-f5c62ce27f75)
![second-game-donkey-kong-window](https://github.com/halfvector/halfvector/assets/1817604/0db68e52-5593-4ba9-87a0-642e7daf42a4)

C++ with meta-programming  
An emulator with CPU, PPU, and input support. Win32 GDI-based rendering. Cycle-accurate emulation, multiple PPU-CPU sync modes. Ran multiple games (like Super Mario and Donkey Kong).  
Development was straightforward thanks to the many freely available and detailed 6502 and RP2A03 CPU references.  

