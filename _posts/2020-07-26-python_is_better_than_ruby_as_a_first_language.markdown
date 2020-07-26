---
layout: post
title:      "Python is better than Ruby (as a first language)"
date:       2020-07-26 17:53:09 +0000
permalink:  python_is_better_than_ruby_as_a_first_language
---

So before I attended the Flatiron SE bootcamp, my only programming experience was teaching myself basic Python. I didn’t have any bias towards Python, I just read online that it was one of the best first languages to learn. And if you research "Best programming languages to learn" today, in 2020, Python is still up there as one of the most popular. And this makes sense: It has a syntax that encourages well-formatted code and best practices, and has a lot of uses. 

So you can imagine my surprise when I learned that Flatiron’s SE bootcamp taught Ruby instead of Python. I remember thinking things like *“Ruby? What the heck is that?”* and *“Can’t Python do everything Ruby can do? Why Ruby?”*. I even went as far as to almost ask why Flatiron taught Ruby instead of Python in my admissions interview, which in retrospect would’ve been pretty disrespectful.

But now, after months of learning the *ins and outs*, the *ups and downs* of Ruby, I, Gavin Sharkey, can confidently say that Python... is still the best first language.

Now I could just end the blog post here and let you take my word at face value, but honestly it doesn't really have much face value. So here are a few reasons why I believe, at least compared to Ruby, Python is the best first language:

#### 1. Python teaches proper indentation and best practices

When first learning how to be a developer, besides learning the basics of variables, iteration, and so on, it's also very important that one learns best practices and proper styling. If you plan on becoming a full-time software engineer, or even just to work with other people on a project, you ***CANNOT*** have ugly, illegible code. No one will want to work with you if they can't even read your code! That's why it's very important to develop good habits when it comes to indentation and styling, as early as possible. Enter Python.

The way Python defines blocks of code is unique, because instead of relying on curly braces (or a do-end block in Ruby), it uses indentation. Indentation becomes a necessity, because Python literally won't work without it! Consider this code:
```
#python
def full_name(first_name, last_name):
    print(first_name + " " + last_name)
		
#ruby
def full_name(first_name, last_name)
  puts "#{first_name} #{last_name}"
end
```
The body of the Python function is what's indented underneath the function defintion. To leave the function body, you just unindent. In Ruby, the body of the function is what's between the function definition and the closing tag (`end` in Ruby, curly braces in most other languages), and the indentation is not enforced. 

This way of writing code that Python enforces is very helpful for a beginner. It develops excellent styling habits very early on, which you will carry into any language you learn later. I sure know I did.

#### 2. Ruby is a little too magical...

Now that I'm pretty familiar with Ruby, there's actually a lot that I love about it. Yes, it's an excellent OOP language with a simple yet powerful ruleset, making it great for scripting. But what I truly love about Ruby is its *methods*, specifically the instance methods for arrays, hashes, and strings. Just take a quick look at the [Ruby built-in Array methods](https://ruby-doc.org/core-2.7.0/Array.html#method-i-26) and you'll be blown away by just how many methods there are.
I think the best example of the magical power of Ruby would be the [Enumerable Module](https://ruby-doc.org/core-2.7.0/Enumerable.html), a collection of methods for arrays and other iterable types, that allow you to do pretty much any sort of data manipulation you could dream of. And this is all standard Ruby!

So this all sounds great right? Ruby sounds awesome! However, here's my problem: Pretty much any other language you learn isn't going to have all these methods. For example, in JavaScript, outside of the more common methods like `map`, `filter`, `sort`, `find`, etc., If you want similar functionality to arrays in Ruby, you'll have to either import some library, or just write the method yourself. I especially felt this when I'd do JavaScript challenges on a site like codewars.com. I'd run into a problem where I had to do some complex manipulation of an array or a string, and all I could think was: "Man, this would be so easy in Ruby...". And JavaScript is pretty high-level! If you're going from Ruby to Java or C++, you'll be in for a wild ride, which leads me to another point about the high-level nature of Ruby...

There's a certain mindset that goes into learning Ruby, that everything is an object. When writing Ruby, you're always instanciating objects, calling methods on objects, etc.. Even when you call a global method, you're actually calling a method on the Kernel object, which most objects inherit from. And don't even get me started on *implicit self*.

This mindset carries over into even basic things like loops and iteration. In Ruby, it's standard to use the `each` method, as opposed to a for loop:
```
#python
for i in range(10):
    print(i)
		
#ruby
(0...10).each do |i|
  puts i
end
```
Which leads me back to Python. Python isn't *low-level* by any means, but it's built-in methods for lists and strings are simple, and more in line with what you'd expect to find in most modern languages. Also, its syntax for loops and iteration is more traditional, and much more reminiscent of loops found in JavaScript and C. Python, I feel, is this sweet spot between the low-level, traditional nature of something like C, and the abstraction and simplification of something like Ruby. Therefore, I feel Python has the edge, as it facilitates a much smoother transition to any future languages you choose to learn, as opposed to Ruby, where you may have to unlearn some of the Ruby mindset.

#### 3. You can do a lot with Python...

I think if you ask most developers what the best use of Ruby is, they'll tell you: "Oh, Rails for sure". If you press them a bit more, they may say "Well, it's a good scripting language too" or "It has uses for data analysis", but Ruby really shines in web development with Rails and Sinatra. And in many ways, that's fine! Ruby on Rails is an excellent MVC web application framework. From how ActiveRecord makes SQL queries and table associations a breeze, to how ActionController makes configuring your routes just as easy as writing basic Ruby classes, Rails makes web development fun. But Rails isn't the only framework...

[Django](https://www.djangoproject.com/) is a web application framework for Python that, essentially, can do everything Rails can do. Sure, they have they're differences, but they solve the same problem. They're both frameworks for simplifying the web application development process, offering abstract, powerful solutions for everything from managing databases to routing. So what's the major difference? Well, Python is more than just Django.

Another area where Python really shines is data science and machine learning. [It recently became one of the most common languages used among data scientists](https://www.kdnuggets.com/2018/05/poll-tools-analytics-data-science-machine-learning-results.html), and that makes sense: There are many third-party Python libraries for data science and analysis, including but limited to: Pandas, NumPy, MatPlotLib, SciPy, and TensorFlow. If you're seeking a carreer in data science/analysis, Python is definitely the language to learn.

This one isn't as big, but you can also make simple games in Python with [PyGame](https://www.pygame.org/wiki/GettingStarted). You won't be making the next Grand Theft Auto with it, but people have made some [pretty cool stuff](https://itch.io/games/made-with-pygame) with it. If you're looking to test the waters of game development but you don't want to learn C++ quite yet, Python isn't a bad place to start.

In conclusion, the diversity of uses and potential careers Python offers puts it a step above Ruby, which is mainly limited to web development.

#### Summary

So that's it! That's why I feel Python is a better first language. However, I would like to make it clear that I am still learning; I'm sure there are plenty of valid counter-arguments to my opinion. If you have a comment, let me know! I'm learning everyday, and I'd love to learn something new. I hope you enjoyed!




 










