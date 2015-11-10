# boost.props
Visual Studio property sheet for [Boost](http://www.boost.org/)

##Use cases
* To keep one single copy of boost on your computer despite having multiple VS projects.
* To compile boost with a compiler other than MSVC.

Otherwise it's probably preferrable to install boost from nuget, see:  
https://www.nuget.org/packages/boost/ (only headers) or  
https://www.nuget.org/packages/boost-vc140/ (compiled)

##Installation
* Add this project as a submodule:  
`git submodule add https://github.com/blole/boost.props`  
or simply download the boost.props file.
* Set the system environment variable `BOOST_ROOT` to where you downloaded boost to, e.g. `C:\lib\boost_1_59_0`
* Restart Visual Studio (so it has the new environment variable)
* Add boost.props to your project in Visual Studio:  
View > Property Manager > right-click your project > Add Existing Property Sheet

Now you can `#include <boost/...>`
