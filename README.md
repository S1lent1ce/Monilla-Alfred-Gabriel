#include <iostream>
using namespace std;
int main() {
     int choice;

    cout << "1. Circle "<<'\n';
    cout << "2. Triangle" << '\n';
    cout << "3. Square" << '\n';
    cout << "=======================" << '\n';
    cout << "Enter your choice (1-3)" << '\n';
    cin >> choice;
    cout << "=======================" << '\n';
      switch (choice) {

      case 1: { double r;
            cout << "enter the radius of the circle: " << '\n';
            cin >> r;
            double p,d,c,a;
            p = 3.14159265359;
            d = 2 * r;
            c = 2 * p * r;
            a = p * r *r;

            cout << "RESULTS: " << '\n';
            cout << "Radius: " << r << '\n';
            cout << "Diameter: " << d << '\n';
            cout << "Circumference: " << c <<'\n';
            cout << "Area: " << a << '\n';
                   break;

      }
      case 2: { double b,h,a;
            cout << "Enter the Base of the Triangle: " << '\n';
            cin >> b;
            cout << "Enter the Heigh OF the Triangle: " << '\n';
            cin >> h;

              a = 0.5 * b * h;
              cout << "RESULTS" << '\n';
              cout << "=======================" << '\n';
              cout << "Area of the Triangle: " << a << '\n';
                    break;
            }



      case 3: { double s;
            cout << "Enter side length: " << '\n';
            cin >> s;

            double a,p,d;

            a = s * s;
            p = 4 * s;
            d = s * 1.41421356237;

            cout << "RESULTS" << '\n';
            cout << "=======================" << '\n';
            cout << "Side: " << s << '\n';
            cout << "Area: " << a << '\n';
            cout << "Perimeter: " << p << '\n';
            cout << "diagonal: " << d << '\n';
                  break;
      }

      default:
        cout << "Wrong Input" << '\n';
      }

     return 0;
}
