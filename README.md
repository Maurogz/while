import javax.swing.JOptionPane;

public class DiarioDeNotas {

    public static void main(String[] args) {
        String Usuario = JOptionPane.showInputDialog("Digite: 1 para Aluno, 2 para Professor");
         String materia = JOptionPane.showInputDialog("Digite a sua Materia");
        String nome = JOptionPane.showInputDialog("Qual seu nome?");
        int i = 1;
        
        switch (Usuario) {
            case "1":
                JOptionPane.showMessageDialog(null,"Bem vindo Aluno " + nome);
                break;
                
                
            case "2":
              
                 while(i<=3){
                    
                   i++;
                 
                JOptionPane.showMessageDialog(null,"Bem vindo Professor " + nome);   
                double nota1 = Double.parseDouble(JOptionPane.showInputDialog(null, "Digite sua nota1"));
                double nota2 = Double.parseDouble(JOptionPane.showInputDialog(null, "Digite sua nota2"));
                double nota3 = Double.parseDouble(JOptionPane.showInputDialog(null, "Digite sua nota3"));
                
                double media = nota1 + nota2 + nota3 /3;
              
                if(media > 70){
                    JOptionPane.showMessageDialog(null,"aprovado");
                   
                }if (media < 70){
                    JOptionPane.showMessageDialog(null,"reprovado");
                }
                 }
                break;
                
            
                    
                 
            default:
                JOptionPane.showMessageDialog(null,"Opção Invalida");
                break;
        }
       
       
         
    }
}
