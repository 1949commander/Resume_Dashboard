# Resume_Dashboard
 Collection of Code Projects
## Introduction

During my last two weeks at the Tech Academy, I worked with a team of peers on a continuing development project to deploy a full scale .NET MVC Web Application using C#. Working on a continuing development project was a great experience requiring multiple skills such as fixing bugs, cleaning up code and adding new features. 

Some of the requested new features requests were significant in size that could have taken a lot of time to create totally from scratch but repurposing public available coding greatly reduced the time to create and debug the new features. I learned how reusing existing work can allow you to deliver a high quality product on schedule. 

Since this web application was already well underway in its development process a significant portion of the basic framework was already in place. However, there were important new features that needed to be completed. We had three stories to complete covering a styling and html, a code first database creation and a scaffolding task for CRUD pages.

This two week sprint gave me significant experience using AZURE to manage and update the Project manager when my Stories were complete and ready for them to merge them to the main branch. I also gained even more experience using Visual Studio. I was able to utilize skills learned during my coursework studies on a full scale Web Application.

Below are descriptions of the stories I worked on, along with code snippets and navigation links. I also have some full code files in this repo for the larger functionalities I implemented.

## Front End Stories
 * [Donation Page](#donation-page)
 
## Back End Stories
* [Code First](#code-first)
* [Meetup API](#meetup-api)

### Donation Page
This Story was to create a UI for the Donations interface which I styled per the customers requirements. The customer wanted an interface that was scalable depending on display size. So the use of Bootstrap Grid System and Fluid Container was used to meet the customers needs. Here is the [code  I created](./Donate.cshtml) to implement the Donate Dashboard shown below.

![Donate Dashboard](https://user-images.githubusercontent.com/61473218/118592558-1a48cc80-b774-11eb-8597-1ddbda188624.png)

### Code First
```C#
using System;
using System.Collections.Generic;
using System.ComponentModel.DataAnnotations;
using System.ComponentModel.DataAnnotations.Schema;
using System.Data.Entity;
using System.Linq;
using System.Web;

namespace TheatreCMS3.Areas.Blog.Models
{
    [Table("BlogPhotos")]
    public class BlogPhoto
    {

        [Key]
        public int BlogPhotoId { get; set; }
        public string Title { get; set; }
        public byte[] Photo { get; set; }
    }
    
}
```


