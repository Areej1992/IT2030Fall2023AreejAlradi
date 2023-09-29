# Week 4 Lab - Debugging the Tip Calculator App

## Error List:

1. **TipCalculator.cs** (Models)
   - Namespace: TipCalculator.Models
   - Class: Calculator
   - Error in line 16: Missed ';'
   - **Error (CS10002):** ';' expected
   - **Fix:** Change `return tip` to `return tip;`

2. **HomeController.cs** (Controllers)
   - Namespace: TipCalculator.Controllers
   - Class: HomeController
   - Error in line 14: Name error (Viewbag)
   - **Error (CS0103):** The name 'Viewbag' does not exist in the current context
   - **Fix:** Change `Viewbag.TwentyFive = 0;` to `ViewBag.TwentyFive = 0;`

3. **HomeController.cs** (Controllers)
   - Namespace: TipCalculator.Controllers
   - Class: HomeController
   - Error in line 15: Missed 'return'
   - **Error (CS0161):** 'HomeController.Index()': not all code paths return a value
   - **Fix:** Change `View();` to `return View();`

4. **Index.cshtml**
   - **Error:** Typo in line 16
   - **Fix:** Change `<label>@ViewBag.Fifteem.ToString("c2")</label>` to `<label>@ViewBag.Fifteen.ToString("c2")</label>`

## Summary:
In this lab, I encountered and fixed the following errors:
- In the `Calculator` class in `TipCalculator.cs`, I added a missing semicolon in line 16.
- In `HomeController.cs`, I corrected a typo in the usage of `ViewBag` and added a missing 'return' statement.
- In the `Index.cshtml` view, I fixed a typographical error.

These corrections resolved the issues and allowed the Tip Calculator app to function correctly.

Note: This is a sample structure for your README.md file. Make sure to format and organize it according to your preference and any specific guidelines provided by your instructor.
