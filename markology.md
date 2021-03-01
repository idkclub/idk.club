<h1>
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="1 1 8 8" width="40" id="arco">
    <title>Markology Logo</title>
    <style>
    #arco polygon {
      display: none;
    }
    #arco:hover g {
      animation: .5s infinite launch;
    }
    #arco:hover polygon {
      animation: .1s infinite flame;
      display: block;
      transform-origin: 5px 6px;
    }
    #arco:hover polygon:nth-of-type(1) {
      animation-delay: -0.01s;
    }
    @keyframes flame {
      50% {
        transform: scale(.9);
      }
    }
    @keyframes launch {
      20% {
        transform: translate(.3px, -.5px);
      }
      40% {
        transform: translate(-.4px, -.6px);
      }
      60% {
        transform: translate(.4px, -.6px);
      }
      80% {
        transform: translate(-.3px, 0);
      }
    }
    </style>
    <g stroke="#0093d3" stroke-linecap="round">
      <circle
        stroke-width=".5"
        cx="5"
        cy="4"
        r="2"
        fill="none"
      />
      <line x1="3.8" y1="6" x2="3" y2="7" />
      <line x1="6.2" y1="6" x2="7" y2="7" />
      <polygon points="5,6 4,7 5,9 6,7" stroke-width="0" fill="orange" />
      <polygon points="5,6 4.2,7 5,8.8 5.8,7" stroke-width="0" fill="red" />
      <path d="M 4 4 A 1 1 0 0 1 5 3" stroke-width=".3" fill="none" />
      <line x1="5" y1="6.3" x2="5" y2="8" />
    </g>
    <a href="/markology" target="_top" id="arco">
      <rect width="10" height="10" fill="transparent" />
    </a>
  </svg>
  Markology
</h1>

![Markology on MacOS and iOS](/assets/markology.png)

<style>
@media (prefers-color-scheme: light){
  img {
    content: url("/assets/markology.light.png");
  }
}
</style>

## What is this?

An opinionated, zettelkasten-inspired note creation and linking tool.

## Supports:

- Markdown (via [Down](https://github.com/johnxnguyen/Down)).
- Offline usage and search (via [GRDB](https://github.com/groue/GRDB.swift)).
- iCloud syncing.

## Why?

- To recall a concept, while only remembering what it related to.
- To organize thoughts, without needing a heirarchy.
- To create and discover interesting connections.
- To track new knowledge, in a way that makes it easy to build on.
