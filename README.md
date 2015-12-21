import javax.swing.ButtonGroup; 
public class Calc extends javax.swing.JFrame {

public Calc() {
    initComponents();
    groupButton();
}
private void groupButton(){
    ButtonGroup bg1 = new ButtonGroup();
    bg1.add(jRadioButton1);
    bg1.add(jRadioButton2);
    bg1.add(jRadioButton3);
    bg1.add(jRadioButton4);
}


@SuppressWarnings("unchecked")
// <editor-fold defaultstate="collapsed" desc="Generated Code">                          
private void initComponents() {

    TXT_1 = new javax.swing.JTextField();
    TXT_2 = new javax.swing.JTextField();
    jRadioButton2 = new javax.swing.JRadioButton();
    Button = new javax.swing.JButton();
    level = new javax.swing.JLabel();
    jRadioButton3 = new javax.swing.JRadioButton();
    jRadioButton4 = new javax.swing.JRadioButton();
    jRadioButton1 = new javax.swing.JRadioButton();

    setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

    jRadioButton2.setText("Substraction");

    Button.setText("OK");
    Button.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            ButtonActionPerformed(evt);
        }
    });

    jRadioButton3.setText("Multiply");

    jRadioButton4.setText("Division");

    jRadioButton1.setText("Addition");

    javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
    getContentPane().setLayout(layout);
    layout.setHorizontalGroup(
        layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
        .addGroup(layout.createSequentialGroup()
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                .addGroup(layout.createSequentialGroup()
                    .addContainerGap()
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                        .addComponent(TXT_1, javax.swing.GroupLayout.PREFERRED_SIZE, 164, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addComponent(TXT_2, javax.swing.GroupLayout.PREFERRED_SIZE, 164, javax.swing.GroupLayout.PREFERRED_SIZE)))
                .addGroup(layout.createSequentialGroup()
                    .addGap(20, 20, 20)
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                        .addComponent(Button)
                        .addComponent(level, javax.swing.GroupLayout.PREFERRED_SIZE, 188, javax.swing.GroupLayout.PREFERRED_SIZE))))
            .addGap(40, 40, 40)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                .addComponent(jRadioButton4)
                .addComponent(jRadioButton2)
                .addComponent(jRadioButton3)
                .addComponent(jRadioButton1))
            .addContainerGap(67, Short.MAX_VALUE))
    );
    layout.setVerticalGroup(
        layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
        .addGroup(layout.createSequentialGroup()
            .addContainerGap()
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                .addComponent(TXT_1, javax.swing.GroupLayout.PREFERRED_SIZE, 49, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addComponent(jRadioButton1))
            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                .addGroup(layout.createSequentialGroup()
                    .addComponent(TXT_2, javax.swing.GroupLayout.PREFERRED_SIZE, 52, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addGap(30, 30, 30)
                    .addComponent(Button)
                    .addGap(38, 38, 38)
                    .addComponent(level, javax.swing.GroupLayout.PREFERRED_SIZE, 53, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGroup(layout.createSequentialGroup()
                    .addComponent(jRadioButton2)
                    .addGap(18, 18, 18)
                    .addComponent(jRadioButton3)
                    .addGap(18, 18, 18)
                    .addComponent(jRadioButton4)))
            .addContainerGap(38, Short.MAX_VALUE))
    );

    pack();
}// </editor-fold>                        

private void ButtonActionPerformed(java.awt.event.ActionEvent evt) {                                       

    if(jRadioButton1.isSelected()){
        String name = TXT_1.getText();
   double number1 = Double.parseDouble(name);
   String name2 = TXT_2.getText();
   double number2 = Double.parseDouble(name2);

   double total = number1+number2;
   String total1= String.valueOf(total);
    level.setText("Total = "+total1);
    }

    if(jRadioButton2.isSelected()){
        String name = TXT_1.getText();
   double number1 = Double.parseDouble(name);
   String name2 = TXT_2.getText();
   double number2 = Double.parseDouble(name2);

   double total = number1-number2;
   String total1= String.valueOf(total);
    level.setText("Total = "+total1);
    }

    if(jRadioButton3.isSelected()){
        String name = TXT_1.getText();
   double number1 = Double.parseDouble(name);
   String name2 = TXT_2.getText();
   double number2 = Double.parseDouble(name2);

   double total = number1*number2;
   String total1= String.valueOf(total);
    level.setText("Total = "+total1);
    }

    if(jRadioButton4.isSelected()){
        String name = TXT_1.getText();
   double number1 = Double.parseDouble(name);
   String name2 = TXT_2.getText();
   double number2 = Double.parseDouble(name2);

   double total = number1/number2;
   String total1= String.valueOf(total);
    level.setText("Total = "+total1);
    }
}                                      

/**
 * @param args the command line arguments
 */
public static void main(String args[]) {
    /* Set the Nimbus look and feel */
    //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
    /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
     * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
     */
    try {
        for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
            if ("Nimbus".equals(info.getName())) {
                javax.swing.UIManager.setLookAndFeel(info.getClassName());
                break;
            }
        }
    } catch (ClassNotFoundException ex) {
        java.util.logging.Logger.getLogger(Calc.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    } catch (InstantiationException ex) {
        java.util.logging.Logger.getLogger(Calc.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    } catch (IllegalAccessException ex) {
        java.util.logging.Logger.getLogger(Calc.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    } catch (javax.swing.UnsupportedLookAndFeelException ex) {
        java.util.logging.Logger.getLogger(Calc.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    }
    //</editor-fold>

    /* Create and display the form */
    java.awt.EventQueue.invokeLater(new Runnable() {
        public void run() {
            new Calc().setVisible(true);
        }
    });
}

// Variables declaration - do not modify                     
private javax.swing.JButton Button;
private javax.swing.JTextField TXT_1;
private javax.swing.JTextField TXT_2;
private javax.swing.JRadioButton jRadioButton1;
private javax.swing.JRadioButton jRadioButton2;
private javax.swing.JRadioButton jRadioButton3;
private javax.swing.JRadioButton jRadioButton4;
private javax.swing.JLabel level;
// End of variables declaration                   

}
