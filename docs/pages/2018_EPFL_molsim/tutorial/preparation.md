Preparation
===========

Start the Quantum Mobile virtual machine, open a terminal window and
type

```bash
workon aiida
```

This activates the virtual environment, in which AiiDA is installed.

Since Quantum Mobile focuses on *ab initio* calculations, it is missing
some aiida plugins we are going to need. Let’s install them (this can
take 3 minutes):

```bash
pip install aiida-raspa aiida-zeopp
```

Before we start creating data ourselves, we are going to look at an
existing AiiDA database. Let’s import one from the web:

```bash
verdi import {{ site.url }}/assets/2018_EPFL_molsim/isotherms.aiida
```