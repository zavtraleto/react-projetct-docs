

# Project organization

```
AxxisAdmin_React/
└── src/
   ├── assets/ 
   ├── components/
   ├── features/
   ├── pages/
   ├── store/
   └── utils/
```

Your project components should be separated in at least three directories.
Each of these directories have special types of components:

### `components/`
Stateless components. Shouldn't store state. Most components in this
directory will be function-based components. Stuff like buttons, inputs,
labels and all presentational components goes here. 

### `features/`
Feature components can store state. Features are built mostly from
the composition of presentational components with some styles to layout
them together. They can dispatch Redux actions when applicable

### `pages/`
Page components can store state, receive route parameters. Pages are the highest level of application's
components. They represent the application routes and most times are
displayed by a router.


Other directories description:

### `assets/`
Here we store our global styling in `styles/` directory, images and icons in `img/` directory and `fonts/` are used as fonts storage.

### `store/`
Here we got our Redux Store core file. Also here we could store shared logic (global selectors etc.)

### `utils/`
Utils are used for global utilities stuff (e.g axios request logic\interceptors). 
Storing global constants and all other stuff that can be global for the project
