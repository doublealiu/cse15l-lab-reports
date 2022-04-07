# Sponge4J
Welcome to the **Sponge4J** library documentation. In this first page, I will give you a conceptual overview of the overall *goals* of Sponge4J as well as some *starter code* to get you hacking away.

## Getting started

In case you live under a rock [SpongeBob](https://en.wikipedia.org/wiki/SpongeBob_SquarePants) (See how his name is CamelCase? He was built for programming!) is a fictional cartoon character (in my opinion the best character ever).

Enjoy this image of spongebob
![Image](https://upload.wikimedia.org/wikipedia/en/4/44/SpongeBob_SquarePants_characters_promo.png)

> I'm ready! I'm ready! I'm ready!

Here is a list of SpongeBob's friends (in no particular order):
- Patrick
- Squidward
- Mr. Krabs

And here is a list of Spongebob's leisure activities (in a particular order)
1. Jellyfishing
2. Work
3. Screaming

This tutorial focuses on the *jellyfishing* functionality of Sponge4J, but there is a lot more you can do with it.

---

Now that we've gone over the conceptual overview of the library, let's get into the code.

We can start with:
```java
SpongeBob spongeBob = new SpongeBob();
spongeBob.catchJellies();
```
To get Spongebob to start catching jellyfish.

For some more advanced jelly catching techniques, we can instantiate the SpongeBob object with a configuration first:

```java
SpongeBobConfiguration config = new SpongeBobConfiguration()
    .eagerness(5)
    .capacity(6)
    .withPatrick();
SpongeBob spongeBob = new SpongeBob(config);
spongeBob.catchJellies();
```

Notice how we use a configuration object and pass it into the constructor of the object that we are configuring. *Why not use a builder?* **Because I said so.**