package tugasprojek;

/**
 *
 * @author LENOVO
 */

import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class tugas4 {
    public static void main(String[] args) {
        // Membuat frame
        JFrame frame = new JFrame("Aplikasi Hitung Sederhana");
        frame.setSize(350, 200);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setLayout(null);

        // Membuat label dan text field untuk angka pertama
        JLabel labelAngka1 = new JLabel("Angka Pertama:");
        labelAngka1.setBounds(20, 20, 120, 20);
        frame.add(labelAngka1);

        JTextField textFieldAngka1 = new JTextField();
        textFieldAngka1.setBounds(140, 20, 150, 20);
        frame.add(textFieldAngka1);

        // Membuat label dan text field untuk angka kedua
        JLabel labelAngka2 = new JLabel("Angka Kedua:");
        labelAngka2.setBounds(20, 50, 120, 20);
        frame.add(labelAngka2);

        JTextField textFieldAngka2 = new JTextField();
        textFieldAngka2.setBounds(140, 50, 150, 20);
        frame.add(textFieldAngka2);

        // Membuat button untuk menghitung
        JButton buttonHitung = new JButton("Hitung");
        buttonHitung.setBounds(100, 90, 100, 30);
        frame.add(buttonHitung);

        // Membuat label untuk menampilkan hasil
        JLabel labelHasil = new JLabel("Hasil: ");
        labelHasil.setBounds(20, 130, 270, 20);
        frame.add(labelHasil);

        // Menambahkan action listener untuk button
        buttonHitung.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                try {
                    double angka1 = Double.parseDouble(textFieldAngka1.getText());
                    double angka2 = Double.parseDouble(textFieldAngka2.getText());
                    double hasil = angka1 + angka2;
                    labelHasil.setText("Hasil: " + angka1 + " + " + angka2 + " = " + hasil);
                } catch (NumberFormatException ex) {
                    JOptionPane.showMessageDialog(frame, "Masukkan angka yang valid!", "Error", JOptionPane.ERROR_MESSAGE);
                }
            }
        });

        // Menampilkan frame
        frame.setVisible(true);
    }
}
<img width="768" height="441" alt="Screenshot 2026-02-11 101159" src="https://github.com/user-attachments/assets/87d4e784-6f8e-4fbd-b4cc-8b4989ebdd6d" />
<img width="639" height="394" alt="Screenshot 2026-02-11 101206" src="https://github.com/user-attachments/assets/9e649aa7-c8ee-4a9c-b653-62d54382d275" />


