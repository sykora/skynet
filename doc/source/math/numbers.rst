====================================================================
 :mod:`math.numbers` -- Basic number theoretic manipulations 
====================================================================

.. module:: math.numbers
    :synopsis: Basic number theoretic manipulations.
.. sectionauthor:: P.C. Shyamshankar <sykora@lucentbeing.com>

This module defines some basic functions required for number theory, such as:

.. function:: digits(n)

    Returns the sequence of digits of the given number ``n``.

.. function:: divisors(n)

    Generates a list of divisors of the given number, including 1 and itself.
    However, it does not generate in ascending order, and must be sorted if
    required.

.. function:: factorial(n)
    
    Computes the factorial of the given number. Factorials are not defined for
    negative or non-integral numbers.

.. function:: gcd(m, n)

    Computes the GCD (Greatest Common Divisor) of the two given numbers.

.. function:: is_palindrome(n)

    Determines if the given number is a palindrome.

    A palindrome is a number which reads the same way, both forwards and backwards.

.. function:: is_prime(n[, s = 25])

    Tests whether or not the given number is a prime number.

    Optionally takes the number of times to run the probabilistic test, the
    defaults should be suitable for most scenarios.

.. function:: is_square(n)

    Tests if the given number is a square number.

.. function:: modular_inverse(a, m)

    Returns the modular inverse of ``a`` with respect to ``m``. Raises
    ValueError if their GCD is not 1, as required.

.. function:: phi(n)

    Returns the Euler Totient function of the given number. ie, ``phi(n)`` is
    the number of positive integers less than ``n`` and relatively prime to
    ``n``.

.. function:: prime_factors(n)

    Generates a sequence of tuples representing the prime factors of the given
    number, and their corresponding exponents.

.. function:: sigma(n[, k = 1])

    Returns the sum of the ``k``th powers of the divisors of ``n``. By default,
    ``k`` is 1, where ``sigma(n)`` is the sum of the divisors of ``n``.

.. function:: tau(n)

    Returns the number of divisors of n. In fact, ``tau(n) == sigma(n, 0)``.

.. function:: xgcd(m, n)

    Computes the GCD ``g`` of the numbers ``m`` and ``n``, as well as two
    numbers ``x`` and ``y`` such that ``m*x + n*y == g``. Returns ``(x, y,
    g)``.

