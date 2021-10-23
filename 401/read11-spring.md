# Spring
* Spring is the most popular application development framework for enterprise Java. 
* Millions of developers around the world use Spring Framework to create high performing,
 easily testable, and reusable code, its an open source Java platform. 
* It was initially written by Rod Johnson and was first released under the Apache 2.0 license in June 2003.

### we can initialize spring with two ways :
1. if you use gradle you can visit Spring Initializr to generate new project with the required dependencies, here is the build gradle file content.



2. manual initialization:
 when we want to manually initialize the project we must follow some steps:
* navigate to https://start.spring.io .
* choose gradle and java as the language . 
* click dependencies and select spring web, thymeleaf, and spring boot devtools.
* click generate.
* Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.

### Create a Web Controller

* HTTP requests are handled by a controller. 

* the controller is identify by the @Controller annotation.



### Spring model attributes
model attributes: they are the pieces of data that can be accessed during the execution of views.

examples of adding attributes to a view in spring MVC:

* Return ModelAndView with model attributes included:

```
@RequestMapping(value = "message", method = RequestMethod.GET)
        public ModelAndView messages() {
            ModelAndView mav = new ModelAndView("message/list");
            mav.addObject("messages", messageRepository.findAll());
            return mav;
        }
```

* Add attribute to Model via its addAttribute method:

```
 @RequestMapping(value = "message", method = RequestMethod.GET)
        public String messages(Model model) {
            model.addAttribute("messages", messageRepository.findAll());
            return "message/list";
        }
```

* Expose common attributes via methods annotated with @ModelAttribute:

```
 @ModelAttribute("messages")
        public List<Message> messages() {
            return messageRepository.findAll();
        }
```




## [BACK](../README.md)