import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JTextField;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class FirstSwing {

    public static void main(String[] args) {
        JTextField tfOne = new JTextField("First Name");
        JTextField tfTwo = new JTextField("Last Name");
        JButton btn = new JButton("Submit");
        JFrame frame = new JFrame();
        JLabel failureLabel = new JLabel("Please enter both first and last names before clicking submit");
        JLabel successLabel = new JLabel("Submitted successfully!");

        frame.setLayout(null);

        tfOne.setBounds(40, 10, 100, 25);
        tfTwo.setBounds(300, 10, 100, 25);
        btn.setBounds(170, 70, 100, 25);
        failureLabel.setBounds(40, 40, 500, 25);
        successLabel.setBounds(40, 40, 200, 25);
        successLabel.setVisible(false); 
        failureLabel.setVisible(false); 
        
        frame.add(tfOne);
        frame.add(tfTwo);
        frame.add(btn);
        frame.add(failureLabel);
        frame.add(successLabel);

        // Functionality of the button
        btn.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                String firstName = tfOne.getText();
                String lastName = tfTwo.getText();

                if (firstName.equals("First Name") || lastName.equals("Last Name")) {
                    failureLabel.setVisible(true);
                    successLabel.setVisible(false);
                } else {
                    String greeting = "Hello, " + firstName + " " + lastName + "!";
                    successLabel.setText(greeting);
                    successLabel.setVisible(true);
                    failureLabel.setVisible(false);
                }
            }
        });

        frame.setSize(450, 500);
        frame.setVisible(true);
    }
}
