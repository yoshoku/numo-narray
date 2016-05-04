# Numo::NArray - New NArray class library for Ruby/Numo (NUmerical MOdule)
under development

## Related Projects
* [Numo::Linalg](https://github.com/masa16/numo-linalg): Linear Algebra library with [LAPACK](http://www.netlib.org/lapack/).
* [Numo::GSL](https://github.com/masa16/numo-gsl): Ruby interface for [GSL (GNU Scientific Library)](http://www.gnu.org/software/gsl/).
* [Numo::FFTE](https://github.com/masa16/numo-ffte): Ruby interface for [FFTE (A Fast Fourier Transform library with radix-2,3,5)](http://www.ffte.jp/).

## Installation
### Ubuntu, Debian
```shell
apt install -y git ruby gcc ruby-dev rake make
git clone git://github.com/ruby-numo/numo-narray
cd numo-narray
gem build numo-narray.gemspec
gem install numo-narray-0.9.0.1.gem
```

## Quick start
An example
```ruby
[1] pry(main)> require "numo/narray"
=> true
[2] pry(main)> a = Numo::DFloat.new(3,5).seq
=> Numo::DFloat#shape=[3,5]
[[0, 1, 2, 3, 4],
 [5, 6, 7, 8, 9],
 [10, 11, 12, 13, 14]]
[3] pry(main)> a.shape
=> [3, 5]
[4] pry(main)> a.ndim
=> 2
[5] pry(main)> a.class
=> Numo::DFloat
[6] pry(main)> a.size
=> 15
```

## numo-array status compared to numpy

https://github.com/masa16/numo-narray/wiki/Numo-vs-numpy

## [NArray Tentative API Document](http://masa16.github.io/numo-narray/narray/frames.html)
