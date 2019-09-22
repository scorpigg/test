## Andrey Nikitin
### Contact Info
* __City:__ Izhevsk
* __Cell-phone number:__ +7 905 875 65 58
* __e-mail:__ scorpigg@yandex.ru

### Summary
Currently, the IT industry is developing very intensively, as a result, IT companies more and more require programmers. But really literate specialists are not so many, since most want everything at once.
My goal is to become a competent and demanded front-end developer, learn to write beautiful, high-quality code and become part of one of the most demanded companies in the world. Let it take a lot of effort and time, but I think it's worth it.

### Skills
* __Front-end development:__ HTML, CSS, JS(+jQuery)
* __Back-end development:__ PHP, MySQL
* __Other:__ Photoshop

### Latest code
```javascript
  $('.saveNewsBtn').on('click', function(){
    var modalNewsTitle = $('#modalNewsTitle').val();
    var modalNewsAuthor = $('#modalNewsAuthor').val();
    var modalNewsDate = $('#modalNewsDate').val();
    var attrID = $('.modalNewsForm').attr('attr-id');
    
    $.ajax({
      url:'ajax.php?action=editNews',
      success:function(data){
        if(data == 'edited'){
          $('.modalNewsForm').hide();
          location.reload();
        }
      },
      data:{
        'newsTitle': modalNewsTitle,
        'newsAuthor': modalNewsAuthor,
        'newsDate': modalNewsDate,
        'newsID': attrID
      }
    }) 
  })

  $('.delNews').on('click', function(){
    var attrID = $(this).closest('.newsBlock').attr('attr-id');
    var news = $(this).closest('.newsBlock');
    $.ajax({
      url:'ajax.php?action=delNews',
      success:function(data){
        if(data == 'deleted'){
          news.hide(300);
        }
      },
      data:{
        'newsID': attrID
      }
    }) 
  })
  ```
### Experience
__Courses:__

* [HTML Academy](https://htmlacademy.ru/profile/id889231): HTML, CSS, JS
* [Codeacademy](https://www.codecademy.com/profiles/scorpik): HTML, CSS
* [BroAcademy](https://broacademy.brolib.ru/): HTML, CSS, JS, PHP, MySQL (from 01.03.2019 till now)

### Education
Izhevsk State Technical University'13 - Mechanical engineering
####English
At the moment, the level of English is __Pre-intermediate__, but every day I improve my knowledge with using sites [Lingualeo](https://Lingualeo.com), [Duolingo](https://duolingo.com).