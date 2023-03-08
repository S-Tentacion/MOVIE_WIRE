
# MOVIE_WIRE

This is a Movies App built using Next.js, React and [The Movie Database (TMDB)](https://www.themoviedb.org/) API. 

## Demo

A [live deployment](https://moviewire.vercel.app/) of this app is available to try it out.


## Installation 

Clone and install the dependencies for `MOVIE_WIRE` locally:

```bash 
  git clone https://github.com/S-Tentacion/MOVIE_WIRE.git
  cd MOVIE_WIRE
  npm install
```

## Quick setup

1. Get your TMDb API key
2. Get your TMDB API read access token
3. Enter the details into the .env.local file
    
## Running locally

* `npm run dev`: dev build
* `npm run build`: production build
* `npm run static-build`: production static build
* `npm run start`: start the project

## Tech Stack

Built with:

* Next.js
* Redux and Redux Thunk
* react-glider
* react-lazyload
* react-modal-video
* react-scroll
* react-select-search
* redaxios
* use-dark-mode
* @artsy/fresnel
* @loadable/component

## next/image

In most cases, I strongly recommend using the [next/image](https://nextjs.org/docs/api-reference/next/image) component for optimizing how you load images. For the MOVIE_WIRE app, there are a few app-specific reasons we currently don't use the component. Using `react-lazyload`, we lazy-load the entire `MovieListItem` component (for example), where elements like the movie name and star ratings don't load until they get near the viewport. This behavior is currently not possible with next/image. In the future, there may be more "Suspense"-y ways of approaching images in React/Next, which would make this type of pattern more first-class. Until then, check out our approach, but you'll likely be otherwise be able to make next/image work for you.
  
  
## Authors

- [@shubham](https://github.com/S-Tentacion)
