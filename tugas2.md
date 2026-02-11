package tugasprojek;

import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
/**
 *
 * @author LENOVO
 */
public class tugas2 extends JFrame { // Ganti Nama Class maasing masing

    public tugas2() { // Ganti Nama Class maasing masing
        // Set judul frame
        setTitle("Tombol Interaktif");

        // Set ukuran frame
        setSize(300, 200);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null); // Agar frame muncul di tengah layar

        // Buat JLabel
        JLabel label = new JLabel("Halo, klik tombol di bawah!");
        label.setBounds(50, 50, 250, 30);

        // Buat JButton
        JButton button = new JButton("Klik Saya");
        button.setBounds(50, 100, 200, 30);

        // Tambahkan ActionListener pada tombol
        button.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                label.setText("Tombol sudah diklik!");
            }
        });

        // Tambahkan komponen ke frame 
        add(label);
        add(button);

        // Set layout menjadi null agar bisa atur posisi manual
        setLayout(null);
    } //Public class di tutup di sini

    public static void main(String[] args) { //Program Utama
        //  Ganti Nama Objek sesuai nama kelas
        tugas2 frame = new tugas2();
        frame.setVisible(true);
    }
}

<img width="508" height="332" alt="Screenshot 2026-02-11 095814" src="https://github.com/user-attachments/assets/e2144853-55e7-4ab6-87f2-367cfd16a460" />
<img width="508" height="332" alt="Screenshot 2026-02-11 095814" src="https://github.com/user-attachments/assets/2cd954cf-0b4a-4bc9-a27e-58e413b5c588" />

