# Terraform Modules the Right Way

## What is a Terraform Module?

Terraform modules, as the name suggests, are like the LEGO bricks of Terraform. Instead of rewriting the same Terraform resources repeatedly, we can bundle them together into a neat package that can also be dynamic—depending on how we approach them.

Think of it as cooking. Why chop the vegetables every single time when you can have a pre-made mix ready to go? It's a great way to keep your Terraform code clean, easy to use, and, most importantly, easy to read.

However, it’s easy to misuse modules and end up making your Terraform code as convoluted as a government tax form, thus defeating the purpose of using a module. In some cases, it might even create procedures that are *manual with extra steps*—the antithesis of automation.

### The Issue

Let’s face it: nobody wants their Terraform code to look like a Jackson Pollock painting—interesting, but utterly incomprehensible. Misusing modules can lead to a tangled mess of dependencies and configurations that make you want to pull your hair out.

## What to Keep in Mind

Now, I’m not a fan of Apple’s anti-customer practices, but there’s a lot to learn from their design philosophy: make complicated things simple and appealing. And yes, this approach is incredibly relevant when creating Terraform modules.

### Design Philosophy: Simplicity and Dynamism

We want our modules to be as simple as a toaster but as dynamic as a Swiss Army knife. The key to achieving this is **default values**.

Imagine you're building a module that other people will use. Your state of mind should be, "I’m going to publish this module online for everyone to use." It should be intuitive, versatile, and foolproof.

Here's the golden rule: **If your module requires more documentation than a microwave manual, it's too complicated.** Your module should have sensible defaults so that it can be used right out of the box, yet be flexible enough to handle specific use cases.

---

By keeping these principles in mind, you’ll create Terraform modules that are not only functional but also a joy to use. Remember, good code is like a good joke: if you have to explain it, it’s not that good. Happy coding!
