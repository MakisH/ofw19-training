# OpenFOAM Workshop 2024 preCICE training slides

- Title: Getting started with OpenFOAM-preCICE for FSI simulations
- Speaker: Jun Chen, University of Stuttgart
- Authors: Jun Chen, Gerasimos Chourdakis + [more](https://www.precice.org/about/)
- Event: 19th [OpenFOAM Workshop](https://openfoamworkshop.org/), Beijing, China
- Date: June 26, 2024

[Start the presentation](https://makish.github.io/ofw19-training/) - [Get the PDF](https://github.com/MakisH/ofw18-training/blob/master/pdf-export/slides.pdf) (pending)

## Build

Follow the instructions on [reveal.js](https://revealjs.com/installation/), or just install Node.js 10.0.0 or later and do:

```bash
npm install
npm start
```

and go to [localhost:8000](http://localhost:8000/) to see the slides.

## Convert to PDF

See section "[Export to PDF](https://revealjs.com/pdf-export/)" in the reveal.js documentation.

[Decktape](https://github.com/astefanutti/decktape) does a marvelous job converting this presentation to PDF. Get the Docker image (see Decktape README) and run (for localhost):

```bash
docker run --rm -t --net=host -v "$(pwd)":/slides astefanutti/decktape generic --key=" " -p 2000 -s 1920x1440 http://localhost:8000 slides.pdf
```

## License & more

- Based on the material of a related training session at the [OpenFOAM Workshop 2023](https://github.com/MakisH/ofw18-training)
- License: [CreativeCommons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
- Based on [reveal.js](https://github.com/hakimel/reveal.js). Template based on the "White" template by Hakim El Hattab.
- The University of Stuttgart logo is part of the corporate identity of the University of Stuttgart.
