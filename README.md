# Introduction

**Empirical: a C++ library to support efficient, reliable, and accessible scientific software**

Empirical is a library of tools for developing efficient, reliable, and accessible scientific software.

Major components of Empirical include:

* a high-level interface to interact with JavaScript and HTML elements when building with Mozilla's Emscripten compiler (from C++ to high-efficiency JavaScript),
* debugging tools to facilitate audited memory management,
* a powerful set of evolution tools for building Artificial Life or Evolutionary Computation software, and
* a wide range of helper tools to streamline common scientific computing tasks such as run-time configuration and data management.

The Empirical library is developed and maintained primarily by the Digital Evolution Laboratory at Michigan State University.

# Relevance

Historically, the Digital Evolution Laboratory has developed Avida digital evolution platform to support experimental work with self-replicating, evolving computer programs.
The software was successively extended to support new experimental treatments and data collection requirements.
Over time, Avida source became increasingly difficult to maintain and extend.
Run-time inefficiencies accumulated, too.

Around 2015, the lab began to shift focus from maintaining a single piece of software to instead developing a common library to support rapid development of software to back individual digital evolution projects.
Indeed, Empirical provides a flexible digital evolution framework, which can interchangeably employ a variety of selection and population structure techniques.
The digital evolution framework can apply to nearly any optimization problem for which a quantitative solution quality metric can be defined.
However, the library also provides virtual hardware implementations to execute evolving computer programs, which are of particular interest to the group.

In addition to digital evolution tools, Empirical provides debugging wrappers for pointers and standard library components, which track and report out-of-bounds accesses and memory leaks.
These wrappers decompose to normal standard library components in non-debug mode, averting performance penalties.

Emscripten, which compiles C++ to JavaScript code that can run client-side in a web browser, also strongly shaped the development of Empirical.
Historically, Emscripten has provided a limited and low-level interface to interact with HTML and Javascript components.
Empirical's web tools provide an object-oriented interface to these components, including faculties for drawing and animation.
The web browser provides an attractive graphical and interactive medium to visualize intermediate states and results of experiments.
Furthermore, web interfaces are near universally accessible, on both mobile and desktop devices --- they provide a unique opportunity to reach a broad lay audience.
Together, Emscripten and Empirical enable full-fledged software to exploit this medium via a lightweight web driver.

# Discussion

Empirical is header-only, encapsulated into the `emp` namespace, and released under the MIT license, so it is simple to incorporate into existing projects.

Empirical employs unit testing via Catch, automated coverage analysis via codecov, code quality analysis via Codacy, and continuous integration via Travis CI.
Documentation generated via Breathe is hosted at readthedocs.io.
Empirical releases are mirrored on Zenodo, where they are assigned a DOI to allow the library to be cited as a scholarly source and archived to ensure long-term reproducibility of scholarly work performed using the library.

# Completion Status

Empirical is under continuous active development to broaden its tool set, accommodate API changes in the Emscripten compiler, and incorporate new methods from the cutting edge of digital evolution.
However, major library components --- including  web, debug, and digital evolution tools --- are stable and actively used in multiple projects, both inside and outside the Digital Evolution Laboratory.

# Contact Information

**Matthew Andres Moreno (`mmore500@msu.edu`)**

Matthew Andres Moreno is a doctoral student at the Michigan State University Department of Computer Science and Engineering working in the Digital Evolution Laboratory.
His research applies digital evolution methods to study major transitions in evolution and the relationship between genetic encoding schemes and evolvability.

**Charles Ofria (`ofria@msu.edu`)**

Charles Ofria is a faculty member of the department of Computer Science and Engineering at Michigan State University, where he leads the Digital Evolution Laboratory and serves as director for the NSF BEACON Center for the Study of Evolution in Action.
He conducts research on evolution in artificial systems and applies the results to problems in computer science and evolutionary biology.
He developed Avida, a software-based research platform consisting of populations of digital organisms used in biological research.
His research has focused more generally on understanding how evolution produces complex traits and behaviors, with the long-term goal of applying these concepts to the evolution of computational intelligence.

# Supporting Material

* The Empirical library source is hosted at [http://github.com/devosoft/Empirical](http://github.com/devosoft/Empirical).
* The Built with Empirical Gallery, which showcases web tools built using Empirical, is hosted at [https://empirical.readthedocs.io/en/latest/BuiltWithEmpiricalGallery/](https://empirical.readthedocs.io/en/latest/BuiltWithEmpiricalGallery/).
