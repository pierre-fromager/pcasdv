# PcaSdv

The idea is to calculate 

* PCA [fr](https://fr.wikipedia.org/wiki/Analyse_en_composantes_principales) (Principal Component Analysis) 
* SVD [fr](https://fr.wikipedia.org/wiki/D%C3%A9composition_en_valeurs_singuli%C3%A8res) (Singular Value Decomposition) 
* LDA [fr](https://fr.wikipedia.org/wiki/Analyse_discriminante_lin%C3%A9aire) (Linear Discriminant Analysis) fisher method

## References

### PCA

 * [Numerical Example](https://www.itl.nist.gov/div898/handbook/pmc/section5/pmc552.htm)
 * [Online Statistics Calculator](https://datatab.net/statistics-calculator/factor-analysis)
 * [Interprétation d'une ACP sur les variables](http://www.jybaudot.fr/Analdonnees/acpvarres.html)
 * [Principal Component Analysis and Linear Discriminant Analysis with GNU Octave](https://www.bytefish.de/blog/pca_lda_with_gnu_octave.html)

### SVD
@todo Wip

### LDA
@todo Wip

## Requirements

* [CMake](https://cmake.org/). 
* C++ compiler, here g++, [howto change it](https://stackoverflow.com/questions/45933732/how-to-specify-a-compiler-in-cmake) in [CMakeLists.txt](CMakeLists.txt). 
* [Alglib](https://www.alglib.net). 
* [Boost lib](https://www.boost.org/). 
* [Octave](https://www.gnu.org/software/octave/) or [Matlab](https://mathworks.com/products/matlab.html).

## Build

```
./build.sh
```

## Run

```
./build/pca
```

## Sample output
```
Fixture 2x12
	Fixture datas (matrix)
	          33	          80
	          33	          82.5
	          34	          100.8
	          42	          90
	          29	          67
	          19	          60
	          50	          77
	          55	          77
	          31	          87
	          46	          70
	          36	          57
	          48	          64
	Covariance (matrix)
	          106.727	          10.1182
	          10.1182	          170.026
	Correlation (matrix)
	          1	          0.0751117
	          0.0751117	          1
	Eigen vectors (matrix)
	          -0.154098	          -0.988056
	          -0.988056	          0.154098
	Eigen values (vector)
	          171.604	          105.149
	Explained variance (%)
		P0 62.0061
		P1 37.9939
	Lda
	          0.988056	          -0.154098

```
## Testing

@todo Wip

```
./build/pca_test
```
