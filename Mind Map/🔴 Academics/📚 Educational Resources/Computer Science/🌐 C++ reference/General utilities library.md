---
tags: [educational-resource/cpp-reference, computer-science/programming-language/cpp, computer-science/programming-language/c, study-note] 
cards-deck: Default::Computer Science
---

# C++ reference

## General utilities library

### Program support utilities

In C++, what is the difference between `exit()` and `main()`? #card
- When one calls `return` in `main()`, destructors will be called for locally scoped objects.
- In contrast, when one calls `exit()`, no destructors will be called for locally scoped objects
	- A.k.a. any objects that you've created in that function will *not* be destroyed.
	- Note that <span class="spoiler">`static`</span> objects will be cleaned up even if you call `exit()`.
	- Note that if you use <span class="spoiler">`abort()`</span>, no objects will be destroyed.
^1680217549244


In C++, how do we specify a directory? #card
- Use two forward slashes like this `//`.
^1680217549250



