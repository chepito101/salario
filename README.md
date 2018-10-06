# salario

package salario;

import java.util.Scanner;
import javax.swing.JOptionPane;

public class Salario extends javax.swing.JFrame {
    float bn, hx, ob,sueldob, res, tH,res2, res3;
    
    public Salario() {
        initComponents();
    }

      @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        buttonGroup1 = new javax.swing.ButtonGroup();
        jScrollPane1 = new javax.swing.JScrollPane();
        txtnombre = new javax.swing.JTextPane();
        jScrollPane2 = new javax.swing.JScrollPane();
        txtdireccion = new javax.swing.JTextPane();
        jScrollPane3 = new javax.swing.JScrollPane();
        txtsueldobase = new javax.swing.JTextPane();
        btncalcular = new javax.swing.JButton();
        jScrollPane4 = new javax.swing.JScrollPane();
        txtresultado = new javax.swing.JTextPane();
        chkbono = new javax.swing.JCheckBox();
        chkhorasextras = new javax.swing.JCheckBox();
        chkotros = new javax.swing.JCheckBox();
        comboLista = new javax.swing.JComboBox<>();
        jLabel1 = new javax.swing.JLabel();
        jLabel2 = new javax.swing.JLabel();
        jLabel3 = new javax.swing.JLabel();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setBackground(new java.awt.Color(153, 153, 255));
        setCursor(new java.awt.Cursor(java.awt.Cursor.DEFAULT_CURSOR));

        txtnombre.setToolTipText("ingrese un nombre");
        jScrollPane1.setViewportView(txtnombre);

        txtdireccion.setToolTipText("ingrese una direccion");
        jScrollPane2.setViewportView(txtdireccion);

        jScrollPane3.setViewportView(txtsueldobase);

        btncalcular.setText("Calcular");
        btncalcular.setToolTipText("calcular sueldo");
        btncalcular.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btncalcularActionPerformed(evt);
            }
        });

        jScrollPane4.setViewportView(txtresultado);

        chkbono.setText("Bono");
        chkbono.setToolTipText("Bono equivalente a 250");
        chkbono.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                chkbonoActionPerformed(evt);
            }
        });

        chkhorasextras.setText("Horas extras");
        chkhorasextras.setToolTipText("horas extras trabajadas");
        chkhorasextras.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                chkhorasextrasActionPerformed(evt);
            }
        });

        chkotros.setText("Otros bonos");
        chkotros.setToolTipText("Otros bonos");
        chkotros.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                chkotrosActionPerformed(evt);
            }
        });

        comboLista.setModel(new javax.swing.DefaultComboBoxModel<>(new String[] { "Seleccione un Dato", "Administrador", "Jefe de Sistemas", "Auditor", "Otro" }));
        comboLista.setToolTipText("Puestos o Cargos");
        comboLista.addItemListener(new java.awt.event.ItemListener() {
            public void itemStateChanged(java.awt.event.ItemEvent evt) {
                comboListaItemStateChanged(evt);
            }
        });
        comboLista.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                comboListaActionPerformed(evt);
            }
        });

        jLabel1.setFont(new java.awt.Font("Tahoma", 0, 14)); // NOI18N
        jLabel1.setText("Nombre");
        jLabel1.addMouseMotionListener(new java.awt.event.MouseMotionAdapter() {
            public void mouseMoved(java.awt.event.MouseEvent evt) {
                jLabel1MouseMoved(evt);
            }
        });

        jLabel2.setFont(new java.awt.Font("Tahoma", 0, 14)); // NOI18N
        jLabel2.setText("Direccion");
        jLabel2.setToolTipText("Ingrese una direccion");

        jLabel3.setFont(new java.awt.Font("Tahoma", 0, 14)); // NOI18N
        jLabel3.setText("Salario Base");

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                .addGap(55, 55, 55)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                    .addGroup(layout.createSequentialGroup()
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                            .addComponent(jLabel1)
                            .addComponent(jLabel2)
                            .addComponent(jLabel3))
                        .addGap(18, 18, 18)
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                            .addComponent(jScrollPane1)
                            .addComponent(jScrollPane2)
                            .addComponent(jScrollPane3, javax.swing.GroupLayout.PREFERRED_SIZE, 137, javax.swing.GroupLayout.PREFERRED_SIZE)))
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(btncalcular)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(jScrollPane4, javax.swing.GroupLayout.PREFERRED_SIZE, 137, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGap(2, 2, 2)))
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, 66, Short.MAX_VALUE)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                    .addComponent(chkbono, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                    .addComponent(chkhorasextras, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                    .addComponent(chkotros, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                    .addComponent(comboLista, 0, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
                .addGap(33, 33, 33))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGap(49, 49, 49)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                    .addComponent(jLabel2)
                    .addGroup(layout.createSequentialGroup()
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                            .addComponent(jScrollPane1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addComponent(jLabel1))
                        .addGap(18, 18, 18)
                        .addComponent(jScrollPane2, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(chkbono, javax.swing.GroupLayout.PREFERRED_SIZE, 23, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGap(18, 18, 18)
                        .addComponent(chkhorasextras)
                        .addGap(15, 15, 15)))
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addGap(18, 18, 18)
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                            .addComponent(jScrollPane3, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addComponent(jLabel3)))
                    .addGroup(layout.createSequentialGroup()
                        .addGap(3, 3, 3)
                        .addComponent(chkotros)))
                .addGap(32, 32, 32)
                .addComponent(comboLista, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(5, 5, 5)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addComponent(btncalcular, javax.swing.GroupLayout.Alignment.TRAILING)
                    .addComponent(jScrollPane4, javax.swing.GroupLayout.Alignment.TRAILING, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addContainerGap(52, Short.MAX_VALUE))
        );

        pack();
    }// </editor-fold>                        

    private void comboListaActionPerformed(java.awt.event.ActionEvent evt) {                                           
           String itemSeleccionado = (String)comboLista.getSelectedItem();
        if("Administrador".equalsIgnoreCase(itemSeleccionado)){
            txtsueldobase.setText("7000");
        }else if("Jefe de Sistemas".equalsIgnoreCase(itemSeleccionado)){
            txtsueldobase.setText("15000");
        }else if("Auditor".equalsIgnoreCase(itemSeleccionado)){
            txtsueldobase.setText("9000");
        }else if("Otro".equalsIgnoreCase(itemSeleccionado)){
            txtsueldobase.setText("5000");
        }
    }                                          

    private void comboListaItemStateChanged(java.awt.event.ItemEvent evt) {                                            
        // TODO add your handling code here:
    }                                           

    private void chkhorasextrasActionPerformed(java.awt.event.ActionEvent evt) {                                               
        // TODO add your handling code here:
    }                                              

    private void chkotrosActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
    }                                        

    public void calculos(){
        
        try{ 
            
             //bono
        if(chkbono.isSelected()){
            bn=250;
            sueldob = Float.parseFloat(txtsueldobase.getText());
            res = bn + sueldob;
            txtresultado.setText(String.valueOf(res));
        }else{
            bn=0;}
        
            // horas extras
        if(chkhorasextras.isSelected()){
            
            hx=800;
            
            
            //horas extras
            hx= (float) (((sueldob / 30)*28)/180);
            res2 = (hx * hx) + sueldob;
            txtresultado.setText(String.valueOf(res2));
            
         }else{
             hx=0;}
         
        
         //otros bonos
         if (chkotros.isSelected()){
             ob=500;
             sueldob = Float.parseFloat(txtsueldobase.getText());
            res3 = ob + sueldob;
            txtresultado.setText(String.valueOf(res3));
         }else{
             ob=0;}
            
        }catch(NumberFormatException e){
            
        }
    }
    
    private void btncalcularActionPerformed(java.awt.event.ActionEvent evt) {                                            
        
           //verificar que los campos no estan vacios
        if (txtnombre.getText().isEmpty() || txtdireccion.getText().isEmpty() || txtsueldobase.getText().isEmpty())
            
        {
            JOptionPane.showMessageDialog(null, "favor llene los valores vacio");
        }
        else
        {
            //el campo tiene texto
        }   
            
        calculos();
    }                                           

    private void chkbonoActionPerformed(java.awt.event.ActionEvent evt) {                                        
        // TODO add your handling code here:
    }                                       

    private void jLabel1MouseMoved(java.awt.event.MouseEvent evt) {                                   
            jLabel1.setToolTipText("ingresar un nombre");
    }                                  

   
    public static void main(String args[]) {
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
            java.util.logging.Logger.getLogger(Salario.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(Salario.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(Salario.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(Salario.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new Salario().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton btncalcular;
    private javax.swing.ButtonGroup buttonGroup1;
    private javax.swing.JCheckBox chkbono;
    private javax.swing.JCheckBox chkhorasextras;
    private javax.swing.JCheckBox chkotros;
    private javax.swing.JComboBox<String> comboLista;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel jLabel3;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JScrollPane jScrollPane2;
    private javax.swing.JScrollPane jScrollPane3;
    private javax.swing.JScrollPane jScrollPane4;
    private javax.swing.JTextPane txtdireccion;
    private javax.swing.JTextPane txtnombre;
    private javax.swing.JTextPane txtresultado;
    private javax.swing.JTextPane txtsueldobase;
    // End of variables declaration                   
}
