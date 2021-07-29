# Random Qoute Generate Vinilla project 

## This project is very simple and straightforward. But  I can learn something through this project. 
### That's what I am learning New  Javascript syntax here .............
> 
1. Array in Object 
<br> 
>
> project  Code 

### Html Code Here ....... 
```
<div class="qoute-project">
          <div class="container">
              <div class="row">
                  <div class="col-lg-8  offset-lg-2">
                      <div class="quote-box  bg-warning"  style="margin:100px 0; padding: 20px 15px;">
                        <div class="text-center">
                            <button class="btn btn-danger btn-lg mb-4  " id="generator">Qoute Generator </button>
                        </div>                        
                          <p  class="lead ">
                          <span><i class="fas fa-quote-left"></i></span>
                          <span id="qoute">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Harum dolore, modi architecto quibusdam, sunt obcaecati nobis iure perferendis officia, culpa dolor! Reiciendis dolore fuga quia obcaecati nihil nobis autem. Nam ullam illo ad officiis possimus sint dolorem, est debitis laboriosam dolore inventore, blanditiis repudiandae et odio alias laborum. Quidem, odio.</span>
                        </p>
                        <p class="sm-text font-weight-bold" id="author">Kamrul hasan </p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
```

<br>
###   Javascript Code Here ...............

```

        let btn =document.getElementById("generator");
        let text = document.getElementById("qoute")
        let author = document.getElementById("author")
        
        let qouteContent = [
            {
                quote:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Harum dolore, modi architecto quibusdam, sunt obcaecati nobis iure perferendis officia, culpa dolor! Reiciendis dolore fuga quia obcaecati nihil nobis autem.",
                author:"kamrul hasan "
            },
            {
                quote:"Lorem ipsum dolor sit amet consectetur, adipisicing elit. Harum dolore, modi architecto quibusdam, sunt obcaecati nobis iure perferendis officia, culpa dolor! Reiciendis dolore fuga quia obcaecati nihil nobis autem.",
                author:"kamrul hasan "
            },
            {
      quote:
        "Life is too short and sweet to be spent by cribbing and complaining about things. Here are some random quotes about the most wonderful gift that we've got",
      author: " Life"
    },
    {
      quote:
        "Humor is richly rewarding to the person who employs it. It has some value in gaining and holding attention. But it has no persuasive value at all",
      author: "John Kenneth Galbraith"
    },
    {
      quote:
        "God save me from my friends. I can protect myself from my enemies.",
      author: "Claude Louis Hector de Villars "
    },
    {
      quote: "The price of anything is the amount of life you exchange for it.",
      author: "David Thoreau"
    },
    {
      quote:
        "Life is like a landscape. You live in the midst of it but can describe it only from the vantage point of distance. ",
      author: "Charles Lindbergh"
    },
    {
      quote:
        "A critic is someone who never actually goes to the battle, yet who afterwards comes out shooting the wounded.",
      author: " Tyne Daly"
    }
        ];

        btn.addEventListener("click", generate)


        function generate(){
            let qouteIndex = Math.floor(Math.random() *qouteContent.length );

            text.textContent = qouteContent[qouteIndex].quote;
            author.textContent = qouteContent[qouteIndex].author;
        }

```
