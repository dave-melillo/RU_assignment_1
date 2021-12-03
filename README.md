# RU_assignment_1

Building NumPy requires the following software installed:

# Python 3.6.x or newer

Please note that the Python development headers also need to be installed, e.g., on Debian/Ubuntu one needs to install both python3 and python3-dev. On Windows and macOS this is normally not an issue.

# Compilers

To build any extension modules for Python, you’ll need a C compiler. Various NumPy modules use FORTRAN 77 libraries, so you’ll also need a FORTRAN 77 compiler installed.

Note that NumPy is developed mainly using GNU compilers and tested on MSVC and Clang compilers. Compilers from other vendors such as Intel, Absoft, Sun, NAG, Compaq, Vast, Portland, Lahey, HP, IBM are only supported in the form of community feedback, and may not work out of the box. GCC 4.x (and later) compilers are recommended. On ARM64 (aarch64) GCC 8.x (and later) are recommended.

## Linear Algebra libraries

NumPy does not require any external linear algebra libraries to be installed. However, if these are available, NumPy’s setup script can detect them and use them for building. A number of different LAPACK library setups can be used, including optimized LAPACK libraries such as OpenBLAS or MKL. The choice and location of these libraries as well as include paths and other such build options can be specified in a site.cfg file located in the NumPy root repository or a .numpy-site.cfg file in your home directory. See the site.cfg.example example file included in the NumPy repository or sdist for documentation, and below for specifying search priority from environmental variables.
--
Cython

```For building NumPy, you’ll need a recent version of Cython.```
