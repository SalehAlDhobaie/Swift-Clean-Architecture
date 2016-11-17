## Swift-Clean-Architecture
Template for Swift Clean Architecture from uncle Bob lecture.

### Clean Code
This Template is derived from the Clean Architecture proposed by Uncle Bob. They share many common concepts such as the components, boundaries, and models.

![http://fernandocejas.com/2015/07/18/architecting-android-the-evolution/](http://fernandocejas.com/wp-content/uploads/2014/09/clean_architecture1.png)

### Architectural reactive approach

![1](https://cloud.githubusercontent.com/assets/4659608/15095669/8564453e-14dc-11e6-8cbc-2afd74c76ddf.png)

### Model-View-Presenter

![1](http://cdn.macoscope.com/blog/wp-content/uploads/2015/12/diagram_2.png)

### Install
To install the Clean Swift Xcode templates, run:

> make install_templates

To uninstall the Clean Swift Xcode templates, run:

> make uninstall_templates


### How to use it

after you install the template by 'makefile' you will find the templates under custome section.

**NOTE** : you might faced an issue after creating UseCase or Service since the service must implemnts the UseCase Prorotcol. in order to fix the issue create a new file with name "UseCase.swift" for implementation just copy and past the following code below : 

```swift

internal protocol UseCase {
    associatedtype Element
    func execute(request : UseCaseRequest) -> Element
    
}


public protocol UseCaseRequest {
    
}

```



### Credit 
* [Raymond](http://clean-swift.com)
* [Android-CleanArchitecture](https://github.com/android10/Android-CleanArchitecture)
* [ActivityCleanArchitecture Template](https://github.com/alhazmy13/ActivityCleanArchitecture_Template)

