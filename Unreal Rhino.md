- Rhino has multiple examples of connecting it to game engine environments called [Rhino.Inside](https://github.com/mcneel/rhino.inside)

## Rhino Inside
- There is an [Unreal Engine example](https://github.com/mcneel/rhino.inside/tree/master/Epic%20Games/UE)
- The Unreal plugin (USharp) that supports the .NET server connection seems to be broken. The Rhino.Inside project is based on a .NET server.  [This blog post](https://discourse.mcneel.com/t/rhino-inside-ue-getting-started/89269) suggest a different .NET server plugin
- There is a[ workshop on how to do it](https://github.com/mcneel/Rhino.Inside-Workshop/wiki)but in [this post](https://discourse.mcneel.com/t/using-rhino-inside-with-grasshopper-in-ue/101607/4)is clear the project is not maintained or working right now

### Trying it out
- Following the instructions [I need to install Visual Studio propper 2017](https://developer.rhino3d.com/guides/rhinocommon/installing-tools-windows/) with the .NET desktop development workload
- [USharp](https://github.com/pixeltris/USharp) is another dependency but it's deprecated which is not super encouraging
- ![Pasted image 20230501170458](media/Pasted%20image%2020230501170458.png)

## Mindesk
- [This group](https://bsl.hku.hk/rhino-to-unreal-bridge-installation/) has some interesting explorations of intersections of unreal and omniverse with Rhino and also fologram
- [Mindesk](https://mindeskvr.com/unreal/) seems to be a good plugin, unsure if I can do bi-directional editing or what is the price

## Speckle
[Speckle Unreal](Speckle%20Unreal.md)

## Other alternatives
[This tutorial](https://www.youtube.com/watch?v=1s_7NwcXLcY)shows how to use excel to link grasshopper with unreal?
[Pixeling](https://github.com/enmerk4r/pixeling) is a project that streams rhino data to unreal
The same creators authored [Swiftlet](https://github.com/enmerk4r/Swiftlet) that enables to receive and send web requests on Grasshopper

### Rhino 3dm
Rhino has many initiatives to communicate with geometry services 
using compute.rhino3d with Unity [tutorial](https://www.youtube.com/watch?v=zUbm83ynn0Q)

[rhino3dm](https://github.com/mcneel/rhino3dm) can be used for example in a [python application like blender](https://discourse.mcneel.com/t/create-cpython-components-using-hops-in-grasshopper/120517/53) but haven't found stuff for unreal 

There are definitely [way more examples with Rhino compute](https://www.google.com/search?q=%22rhino+compute+server%22+%22unity%22&ei=s6ZSZOe1F4zDkPIP_IGL8AQ&ved=0ahUKEwin25rB4tn-AhWMIUQIHfzAAk4Q4dUDCBA&uact=5&oq=%22rhino+compute+server%22+%22unity%22&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAzIFCCEQoAE6CggAEEcQ1gQQsAM6BQghEKsCSgQIQRgAUKkIWPEMYPkOaANwAXgAgAFSiAHxApIBATWYAQCgAQHIAQLAAQE&sclient=gws-wiz-serp) with Unity than with Unreal 