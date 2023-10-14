# Class 09

## Readings: Ten Thousand 4

## Sources
- [How to Build a Bot and Automate your Everyday Work](https://www.freecodecamp.org/news/building-bots/)
- [Monkey Patching in Python](https://medium.com/@bits_code/https-medium-com-bits-code-monkey-patching-in-python-9a28dc0cbe4f)
- [ChatGPT](https://chat.openai.com/c/3f97b947-22d1-4f22-af06-f271e36190ce)

## Bookmark and Review
- [How to Test Printed Output in Python with Pytest and its Capsys Fixture](https://pavolkutaj.medium.com/how-to-test-printed-output-in-python-with-pytest-and-its-capsys-fixture-161010cfc5ad)

## Reading Questions
<ol>
<li>Describe the types of automation in Python to automate everyday tasks. What are some possible applications of this knowledge in the real-world context?</li> Simple automation are short set of scripts that complete a simple task such as cleaning up or reorganizing file directories. Public API automations utilize HTTP requests to APIs. The text example is an automated watering script for a smart garden. API Reverse Engineering duplicates human behavior and mainly come in the form of bots

<li>What is monkey patching in Python? Discuss its benefits and potential risks. Provide an example where monkey patching can be beneficial.</li> Monkey patching is a technique to update the behavior of a piece of code at run-time. It's great for testing mock behavior of libraries, modules, etc. The risk is accidentally overriding the original code. 

<li>How can you use Pytest and its Capsys fixture to test printed output in Python? Can you describe a situation where this technique would be particularly useful?</li> 

According to ChatGPT...

 To test printed output in Python, you can use Pytest, which is a popular testing framework. Pytest provides a built-in fixture called `capsys` that can be used to capture and inspect printed output. Here's an example of how you can use it:

```python
# test_example.py
def my_function():
    print("Hello, World!")

def test_my_function(capsys):
    my_function()
    captured = capsys.readouterr()
    assert captured.out == "Hello, World!\n"
```

In this example, the `test_my_function` test captures the printed output of the `my_function` using the `capsys` fixture. The `readouterr` method of `capsys` captures the output and returns a tuple containing the captured standard output and standard error. You can then assert the expected output with `captured.out`.

Using the `capsys` fixture is particularly useful in situations where you need to ensure that certain functions print the correct output. This is especially helpful when you're testing functions that interact with the console or produce text-based output. Some scenarios where this technique is useful include:

1. Testing functions that format and print data or messages to the console.
2. Verifying that certain error messages or warnings are correctly displayed.
3. Ensuring that logging functions produce the expected output.

By using the `capsys` fixture in Pytest, you can effectively test the behavior of your functions that involve printing without cluttering the console during the test execution. This allows you to assert the output and ensure that the functions are working as intended.