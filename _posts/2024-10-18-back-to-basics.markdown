---
layout: post
title: "Back to Basics"
categories: blog
---

# Back to Basics

It's been a minute since the last time I worked with React, so today I'm revisiting the fundamentals in preparation for a big project I'm planning.

## What the heck is Vite?

Maybe I'm dating myself, but the last time I built a React project I just used `npm create-react-app` and went about my business. That's not how it's done these days.

There's a new tool on the block called Vite and it makes life as a frontend developer easier. It was originally built for Vue, but luckily it's platform agnostic and can be used with React as well.

How does it make life easier? Good question.

- Magic
- Hot Module Replacements
- and more!

Like I said, good question. I'll report back when I experience some of the benefits first hand. For now, Vite is the recommended way to go so I'm just following best practices here.

## Ah yeah, the fundamentals

Opening up a Vite-made React app brought back a lot of memories of working with regular old vanilla React.

- Components: just functions that return some JSX, which gets compiled to HTML by Babel.

The cool thing about JSX is that you can render JavaScript inside it by putting the JS that you want executed inside of curly brackets.

```JavaScript
const App = () => {
  const name = "Walter White"
  return (
    <div>
      <p>Hello {name}</p>
      <p>I am the one who knocks.</p>
    </div>
  )
}
```

- Props: provide some data to your Components

```JavaScript
const Hello = (props) => {
  return (
    <div>
      <p>Hello {props.name}</p>
    </div>
  )
}

// the name could be passed in as a prop, like this
// props are passed to the component when the component gets called
<Hello name="Walter White" />
```

Neato.
