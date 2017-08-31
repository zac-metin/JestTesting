# JestTesting
Learning testing with Jest

-Only runs test related to changed code
-Snapshot testing
- Helpful Error messages
- Mocks and Spies

# Testing Types

Unit testing: small module or function, testing a small part of your code.

Interaction testing: Confirm interactions work, Assert a function is called on click, message displays, no browser required (Enzyme)

Structural Testing: Validates HTML output. Takes a picture of components output, snapshot testing. Jest saves copy of output with given input, tests break when output changes.

Style Testing: Testing CSS.

# Testing Methods

Assertion Library - A way to declare what you expect

expect(2+2).toEqual(4)

Jest has assertions built in, in expect style.

Helper Libraries - Enzyme core helper library, interaction tests, simulate clicks, dom queries.

react-test-renderer: to render Jest snapshots.

Use JSDOM to run in-memory DOM, inbuilt in Jest.

Centralized vs Alongside test file placement.

# Unit Testing With Jest

describe('Progress Bar', () => {
  test('testname', () => {
      const wrapper = shallow(<Component prop=prop />)
      const expected = wrapper.instance().functionTested()
      expect(expected).toEqual(actual)
    })
  })
