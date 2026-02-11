package tugasprojek;

/**
 *
 * @author LENOVO
 */

import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class tugas3 {
    public static void main(String[] args) {
        // Membuat frame
        JFrame frame = new JFrame("Form Input Nama");
        frame.setSize(300, 150);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setLayout(null);

        // Membuat label
        JLabel label = new JLabel("Masukkan Nama:");
        label.setBounds(20, 20, 120, 20);
        frame.add(label);

        // Membuat text field
        JTextField textField = new JTextField();
        textField.setBounds(140, 20, 120, 20);
        frame.add(textField);

        // Membuat button
        JButton button = new JButton("Submit");
        button.setBounds(100, 60, 80, 30);
        frame.add(button);

        // Menambahkan action listener untuk button
        button.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                String nama = textField.getText();
                JOptionPane.showMessageDialog(frame, "Halo, " + nama + "!");
            }
        });

        // Menampilkan frame
        frame.setVisible(true);
    }
}package tugasprojek;

/**
 *
 * @author LENOVO
 */

import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class tugas3 {
    public static void main(String[] args) {
        // Membuat frame
        JFrame frame = new JFrame("Form Input Nama");
        frame.setSize(300, 150);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setLayout(null);

        // Membuat label
        JLabel label = new JLabel("Masukkan Nama:");
        label.setBounds(20, 20, 120, 20);
        frame.add(label);

        // Membuat text field
        JTextField textField = new JTextField();
        textField.setBounds(140, 20, 120, 20);
        frame.add(textField);

        // Membuat button
        JButton button = new JButton("Submit");
        button.setBounds(100, 60, 80, 30);
        frame.add(button);

        // Menambahkan action listener untuk button
        button.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                String nama = textField.getText();
                JOptionPane.showMessageDialog(frame, "Halo, " + nama + "!");
            }
        });

        // Menampilkan frame
        frame.setVisible(true);
    }
}

<img width="489" height="288" alt="Screenshot 2026-02-11 100311" src="https://github.com/user-attachments/assets/ff6fc7b3-db63-4bc7-9bf7-5507ae93978d" />
<img width="600" height="322" alt="Screenshot 2026-02-11 100320" src="https://github.com/user-attachments/assets/12d0715d-43b9-4a8d-a16f-85ba0caa501c" />

