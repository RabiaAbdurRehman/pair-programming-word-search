# Pair Programming: Word Search

This challenge comes with some initial (buggy!) code. We suggest approaching this problem with a TDD mindset, meaning "write tests, make the tests pass, repeat!".

Start by forking this repository, and cloning your fork. Then, run `npm install` in the directory to install all the dependencies. This project has Mocha for running tests, and you'll find that there are already some tests present.

Run tests with `npm test`. You'll find that one of the tests doesn't pass yet, so you'll want to start by editing the code in `wordsearch.js` to allow the tests to pass.

When the present tests are successful, ask yourself, "Do the current tests cover all the possible cases?" What about the case where the word matrix is an empty array? What if the word is written _vertically_, not horizontally? You'll have to write tests for these cases (and any others that you think of), and you might also have modify the `wordSearch` function to make those new tests pass.
original matrix
[
      ['A', 'W', 'C', 'F', 'Q', 'U', 'A', 'L'],
      ['S', 'E', 'I', 'N', 'F', 'E', 'L', 'D'],
      ['Y', 'F', 'C', 'F', 'Q', 'U', 'A', 'L'],
      ['H', 'M', 'J', 'T', 'E', 'V', 'R', 'G'],
      ['W', 'H', 'C', 'S', 'Y', 'E', 'R', 'L'],
      ['B', 'F', 'R', 'E', 'N', 'E', 'Y', 'B'],
      ['U', 'B', 'T', 'W', 'A', 'P', 'A', 'I'],
      ['O', 'D', 'C', 'A', 'K', 'U', 'A', 'S'],
      ['E', 'Z', 'K', 'F', 'Q', 'U', 'A', 'L'],
    ]
after the transpose()
[
  ['A', 'S', 'Y', 'H', 'W', 'B', 'U', 'O', 'E'],
  ['W', 'E', 'F', 'M', 'H', 'F', 'B', 'D', 'Z'],
  ['C', 'I', 'C', 'J', 'C', 'R', 'T', 'C', 'K'],
  ['F', 'N', 'F', 'T', 'S', 'E', 'W', 'A', 'F'],
  ['Q', 'F', 'Q', 'E', 'Y', 'N', 'A', 'K', 'Q'],
  ['U', 'E', 'U', 'V', 'E', 'E', 'P', 'U', 'U'],
  ['A', 'L', 'A', 'R', 'R', 'Y', 'A', 'A','A'],
  ['L','D','L','G','L','B','I','S','L']
]
after the map() method
[
  'AWCFQUAL',
  'SEINFELD',
  'YFCFQUAL',
  'HMJTEVRG',
  'WHCSYERL',
  'BFRENEYB',
  'UBTWAPAI',
  'ODCAKUAS',
  'EZKFQUAL'
]