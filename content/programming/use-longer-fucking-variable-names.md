---
title: "Use Longer Fucking Variable Names"
date: "2022-04-15"
draft: false
categories: ["programming"]
tags: ["variables", "software developer", "golang", "go"]
summary: Just do it
---

Really, please just do it. I see this crap in so many different repos, written by otherwise amazingly good developers. A recent [Go](https://go.dev/) example:

----

```go
p, err := picFunc()
```

----

What the hell am I supposed to do with this? You know that computers have multiple terabytes of storage now right? What's the bullshit excuse for just using `e`?

----

*I'm saving storage space*

----

You aren't programming the goddamn space shuttle, it's a bot that posts cat pictures on Instagram. You can spare a couple megabytes on your source code files.

----

```go
pic, err := picFunc()
```

----

Okay better, but what's the pic?

----

*The pic from the function*

----

Just pretend I don't know what you're talking about, and imagine me asking you "what the hell are you talking about?".

----

```go
thePicFromThePicFunc, err := picFunc()
```

----

...

----

*I don't understand what you want from me*

----

Try to consider some descriptions of the object that the variable is pointing to. Imagine I'm constantly asking you what the variable is for, how it can be used, and why you need it.

----

```go
thePicFromThePicFuncThatHoldsAPicToUseForLater, err := picFunc()
```

----

Okay, let's maybe just concentrate on **what** a `pic` is. A `picture`? What kind of one?

----

```go
catPicture, err := picFunc()
```

----

Great! What's the context around the cat picture? What info would help me figure out what I can do with the cat picture?

----

```go
latestCatPicture, err := picFunc()
```

----

I'm so proud.

----

*What about `err`?*

----

You name that anything else and I think the Go gopher will manifest itself from your screen and slap you across the face.

## And Write More Comments While You're At It

They're easy, I promise. Write an algorithm that looks weird? Just tell me why it has 19 nested for loops. Don't assume I'll figure it out or read the docs or some other ridiculous assumptions.

```go
// Assigns a variable and and error from calling picFunc()
p, err := picFunc()
```

Go fuck yourself.
