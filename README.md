# kreisberechnung
calculating the circle Area and perimeter
# Der Umfang und Kreisfläche berechnung mit #JOptionPane

import javax.swing.JOptionPane;
 
public class Kreisberechnung {
    public static void main(String[] args) {
        // Aufforderung eine Eingabe zu tätigen
        String radiusInput = JOptionPane.showInputDialog("Geben Sie den Radius des Kreises ein");
 
        double radius = Double.parseDouble(radiusInput);
 
        double flaeche = Math.PI * Math.pow(radius, 2);
 
        double umfang = 2 * Math.PI * radius;
 
        JOptionPane.showMessageDialog(null, "Der Umfang ist: " + Math.round
        (100.0 * umfang)/100.0 + "cm \nDie Kreisfläche ist " + Math.round(100.0 * flaeche)/100.0 + "cm");
    }
   
}
