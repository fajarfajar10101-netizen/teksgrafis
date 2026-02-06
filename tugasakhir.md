
<img width="603" height="297" alt="Screenshot 2026-02-06 085425" src="https://github.com/user-attachments/assets/18515cd1-89c9-497e-aa72-133c84bfaa37" />
<img width="627" height="300" alt="Screenshot 2026-02-06 085436" src="https://github.com/user-attachments/assets/797efc7b-90a5-4ed4-b3c8-70dbcae9680c" />
<img width="645" height="294" alt="Screenshot 2026-02-06 085456" src="https://github.com/user-attachments/assets/ca000a71-1bbc-42b1-9a49-966706a1c8bf" />
<img width="520" height="277" alt="Screenshot 2026-02-06 085503" src="https://github.com/user-attachments/assets/367ca5f6-26a3-4d0e-b7cd-566de0da0ef7" />



package tugasprojek;
import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

/**
 *
 * @author LENOVO ID
 */

public class Tugas5 {
   public static void main(String[] args) {
        JFrame frame = new JFrame("Aplikasi Login Sederhana");
        frame.setSize(350, 200);
        frame.setLayout(null);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        JLabel lblUser = new JLabel("Username:");
        lblUser.setBounds(30, 30, 100, 25);
        frame.add(lblUser);

        JTextField txtUser = new JTextField();
        txtUser.setBounds(130, 30, 150, 25);
        frame.add(txtUser);

        JLabel lblPass = new JLabel("Password:");
        lblPass.setBounds(30, 70, 100, 25);
        frame.add(lblPass);

        JPasswordField txtPass = new JPasswordField();
        txtPass.setBounds(130, 70, 150, 25);
        frame.add(txtPass);

        JButton btnLogin = new JButton("Login");
        btnLogin.setBounds(130, 110, 80, 30);
        frame.add(btnLogin);

        // 5. Logika Validasi (Percabangan if-else)
        btnLogin.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                String username = txtUser.getText();
                String password = String.valueOf(txtPass.getPassword());

                if (username.equals("Fajar22") && password.equals ("2711"
                        + "")) {
                    JOptionPane.showMessageDialog(frame, "Login Berhasil");
                } else {
                    JOptionPane.showMessageDialog(frame, "Login Gagal", "Peringatan", JOptionPane.ERROR_MESSAGE);
                }
            }
        });

        frame.setVisible(true);
    }
}  

