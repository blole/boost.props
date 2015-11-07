# boost.props
Visual Studio property sheet for [Boost](http://www.boost.org/)

##Do I need it?
If you're only going to use header-only boost libraries, you could just download it to your project from nuget, see
https://www.nuget.org/packages/boost/

However, if you need to compile boost, or don't want to download it once for every solution, this could be your solution.

##Installation
* Add this project as a submodule:  
`git submodule add https://github.com/blole/boost.props`  
or simply download the boost.props file.
* Set the system environment variable `BOOST_ROOT` to where you downloaded boost to, e.g. `C:\lib\boost_1_59_0`
* Restart Visual Studio (so it has the new environment variable)
* Add boost.props to your project in Visual Studio:  
View > Property Manager > Right-click your project > Add Existing Property Sheet

Now you can `#include <boost/...>`
