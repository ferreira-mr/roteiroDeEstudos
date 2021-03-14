# Book: Testing Python - David Sale

## Chapter 01 - A History of Testing

This introductory chapter provided a brief description of whom this book is for. By now you should have a Geel for the concept sand topics that are conveyed in subsequent chapters. You were introduced to the subject of testing and give a brief background in the history of testing. You were shown hoe it has evolved from merely an afterthought of the product to a precess. Which in many cases is now baked in to the development of a developer’s  work and is won to produce better results, especially in terms of aiming for zero devotes in production. You liked into why testing is now such a pivot process and how it can benecifgcal both in a trem and lone developer environment.

Finally, the chapter closes by ensuring you have some o the essential tooling on you machine , be it Linux, or Windows or Mac. By getting there fundaments ready, you will be set to take on the examples and ideias in this book and it should as help you in your next projects and beyond.

## Chapter 02 - Writing Unit Tests

### Useful Method in Unit Testing

```python
def test_assert_equal(self):
    self.assertEqual(1, 1)

def test_assert_almost_equal_delta(sel1f):
    self.assertAlmostEqual(1, 1.2, delt=0.5)

def test_assert_raises(self):
    self.assertRaises(ValueError, int, "a")

def test_assert_doc_contains_subset(self):
    expected = {'a': 'b'}
    acutal = {'a': 'b', 'c': 'd', 'e': 'f'}
    self.assertDictEqual(expected, actual)

def test_assert_dict_equal(self):
    expected = {'a': 'b', 'c': 'd'}
    actual = {'c': 'd', 'a': 'b'}

def test_assert_true(self):
    self.assertTrue(1)
    self.assertTrue('Hello, World!')

def text_assert_false(self):
    self.assertFalse(0)
    self.assertFalse('')

def test_assert_geater(self):
    self.assertGreater(2, 1)

def test_assert_greater_equal(self):
    self.assertGreaterEqual(2, 2)

def test_assert_in(self):
    self.assertIn(1, [1,2,3,4,5])

def test_assert_is_instance(self):
    self.assertInsInstance(1, int)

def test_assert_is_not_instance(self):
    self.assertIsNotInstance(1, str)

def test_assert_is_none(self):
    self.assertIsNone(None)

def test_assert_is_not(self):
    self.assertIsNot([], [])

def test_assert_is_not_none(self):
    seld.assertIsNotNome(1)

def test_assert_less(self):
    self.assertLess(1, 2)

def test_assert_less_equal(self):
    self.assertLessEqual(2, 2)

def test_assert_items_equal(self
    self.assertItemsEqual([1, 2, 3], [3, 1, 2])

def test_assert_raises(self):
    self.assertRaises(IndexError, [].pop, 0)
```

You got down to business in this chapter. You were introduced to the concept fo unit testing breaking down your application into small bite-sized chunks that could be tested in isolation. You wrote your first unit test! By taking a small example application such as a Calculator, you were able to see how to test the individual responsibilities of the class and methods.

You wrote unit test that make use of the two main assertions in assertEqual and assertRises to check happy and unhappy paths trohoug the code. PEP-8 showed Python developers the starnds they shoud adhrer to boht in code and in test. By follwing the guidelinw outline in the PEP-8 document, you can ensure you will write neat, redable Python code that is easily accesible to other Python developer.

A comprehensive guide to the diffentes assertion mehots available when unit testin should prove to be a valuable resorce to those starting out or brushing up their skills un unit testing. A clear guide to the method names and arguments to be provided makes it easy to get writing unit tests of your own and also maybe discover some methods you weren't aware of.

Finally, I rounded off the chapter with adives on the standard structure and makeup of a typicla Python application and its test. As with PEP-8, following a standard structure esures it is easier to work on projects with other Python dvelopers, but it is important to do what is best for you and your project should the need arise. Some more advanced unit test cases an improvements complet the chapter to ensure you have eveything you nedd to write good unit tests that exercise you application efficiently.
