# jakobs
Max eines Arrays Inhalt
package schleifen;

public class Maximum {

  /**
   * Bestimmt den größten Wert (Maximum) in einem int-Array.
   *
   * @param a Das int-Array, in dem das Maximum gesucht wird (darf nicht leer sein).
   * @return Der größte Wert, der im Array vorkommt.
   */

  public static int max(int[] a) {
    int m = a[0];               // Startwert: erstes Element

    for (int i = 1; i < a.length; i++) {   // i ist der Index
      if (a[i] > m) {
        m = a[i];
      }
    }

    return m;
  }

  /**
   * liefert das Ergebnis aufm Bildschirm.
   *
   * @param args wird nicht verwendet
   */
  public static void main(String[] args) {
    int[] test = {1, 2, 4, 8};
    System.out.println(max(test)); // sollte 8 ausgeben

    int[] test2 = {5, -3, 12, 7};
    System.out.println(max(test2)); // sollte 12 ausgeben
  }

}
