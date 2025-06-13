# Chef-in-his-Office

This C++ program calculates the **total number of working hours in a week** for multiple test cases, based on a schedule where:

* Chef works **X hours from Monday to Thursday** (4 days),
* and **Y hours on Friday** (a "chill" day with fewer hours),
* with Saturday and Sunday off.

---

### 🔍 Line-by-line Explanation:

```cpp
#include <iostream>
using namespace std;
```

* Includes the standard input/output stream library.
* Allows using `cin` and `cout` without writing `std::` every time.

---

```cpp
int main() {
    int T;
    cin >> T;
```

* `T` is the number of test cases.
* Reads the number of test cases from input.

---

```cpp
    while (T--) {
        int X, Y;
        cin >> X >> Y;
```

* Loops `T` times.
* For each test case, reads two integers:

  * `X`: hours worked each day from Monday to Thursday.
  * `Y`: hours worked on Friday.

---

```cpp
        int total_hours = (4 * X) + Y;
        cout << total_hours << endl;
```

* Calculates total weekly hours:

  * `4 * X` (Mon–Thu) + `Y` (Friday).
* Prints the result on a new line.

---

```cpp
    }

    return 0;
}
```

* Ends the loop and the program.

---

### 🧪 Example:

Input:

```
3
10 5
12 2
8 7
```

Output:

```
45
50
39
```

This C++ program calculates weekly working hours based on input values for multiple test cases. For each test case, it reads two integers: X, the number of work hours from Monday to Thursday (4 days), and Y, the work hours on Friday (a lighter day). It computes the total hours as 4 * X + Y and prints the result for each test case.

The program begins by reading the number of test cases T, then loops through each case, performing the calculation and outputting the result. It's a simple and efficient way to determine weekly work hours based on a fixed schedule, assuming Saturdays and Sundays are holidays.
