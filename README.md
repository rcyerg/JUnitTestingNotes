# JUnitTestingNotes

WHAT IS A UNIT TEST

    + Just code in a test class

    + Executes target code

    + Wants to test a small unit of code works as expected

    + Sometimes exercises target code in several classes at once. Called COMPONENT TESTS

    + Test code obtains the results of the target code and confirms that those results are correct
    that what the code was expect to do was what the code actually did

    + Expected, actual

    + assertions.


    BENEFITS OF UNIT TESTING

    + Provides quick feedback if code is correct, behaves as expected. Don't have to wait
    unit entire system is built.

    + Automated regression checking

    + Design aid. If it's confusing to build the test, it will probably be confusing to utilize
    later on.

    + Improves confidence as a programmer when using that system. Effective for refactoring

    + Acts a form of documentation



    SET UP > EXECUTE > VERIFY : common pattern within any kind of automated test.



    VARIOUS ASSERTIONS:

    + Assert same: verifies that both variables point to the same location in memory. Good for testing enums

    + Assert not same: good for testing when an object is copied to another object isn't the same instance as the one
    it was copied from.

    + Assert true and false, true and false


    Collection Assertions

    + If you use an assert equals to check collections, JUnit will check that the two collections contain equivalent objects
    using the equals method on each of those objects AND that each of those objects are in the same order.

    Collection specific assertion: assertIterableEquals

    + For use when comparing collections of different types.


    SETTING UP AND TEARING DOWN TESTS

    Test Lifecycle Annotations:

    + @BeforeAll
    At the class level, so are static. Can be overridden but usually needs to be static.

    + @BeforeEach

    + @AfterEach

    + @AfterAll
    At the class level, so are static. Can be overridden but usually needs to be static.
