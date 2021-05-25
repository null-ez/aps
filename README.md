# APS
Hi guys i need some help, I am trying to compile this code at Eclipse but having issues. I speak portuguese, hindi, english.

import javax.swing.JOptionPane;

public class CalculaProduto extends Produtos{//classe filha
	}
 
public double CalculaProduto(int opcao) {//metodo calcula produto
	 }

 if(opcao==1) {//escolher primeira opção
	 system.out.println("Torneira")
	 Minutos();
 }
 
torneira= 16*minuitos;//calculando litros
JOptionPane.showMessageDialog(null,"Com"+minutos+"
minutos você acaba gastando cerca de"+torneira+" "litros de Agua por dia",
     "Torneira",

 JOptionPane.INFROMATION_MESSAGE);

     calLitros(torneira);
    } 
    else if (opcao==2) {//escolher segunda opção
   	 system.out.println("Chuveiro")
   	 Minutos();
   	chuveiro= 9*minuitos;//calculando litros
   	JOptionPane.showMessageDialog(null,"Com"+minutos+"
   	minutos você acaba gastando cerca de"+chuveiro+" "litros de Agua por dia",
   	     "Chuveiro",
 JOptionPane.INFORMATION_MESSAGE);
   	calLitros(chuveiro);
    }
    
    else if (opcao==3) {//escolher terceira opção
      	 system.out.println("Descarga")
      	 Descarga();
      	chuveiro= 6*minuitos;//calculando litros
      	JOptionPane.showMessageDialog(null,"Com"+minutos+"
      	minutos você acaba gastando cerca de"+descarga+" "você acaba gastando cerca de "+litros+" litros por dia",
      	     "Descarga",
    JOptionPane.INFORMATION_MESSAGE);
      	calLitros(litros);
      	   	
    	
    }
    else//caso a opção escolhida não seja válida
    	JOptionPane.showMessageDialog(null,"Opção invalida",
    	      	     "Opção Inválida",
    	    JOptionPane.INFORMATION_MESSAGE);
    	      	return opcao;
    	      	}
}

Códigos da classe "excecao":
	
	import javax.swing.JOptionPane;


public class Execao {
	public int tratar(String opt) {//métodos para exeção opção
		int b = 0;
		int teste;
		try {
			  teste=integer.parselnt(opt); //tentando converter
			  b=1;
		}
		catch(numberFormatException n){//caso a conversão não seja possivel
			 JOptionPane.showMessageDialog(null,"Erro no programa,tente denovo.",
					               "Erro no programa",
JOptionPane.WARNING_MASSAGE);
			    System.out.println("");
		}
		return b;
	}
	public int tratarmin(String min) {//método para exeção minutos
		int b= 0;
		double teste;
		try {
			  teste= Double.parseDouble(min);//tentando converter
			  b=1;
		}
		catch(NumberFormatException n) {//caso a conversão não seja possivel
			
       JOptionPane.showMessageDialog(null,"erro no programa,tente novamente."
    		                       "Erro no programa",
 JOptionPane.WARNING_MESSAGE);
       
		}
		
		return b;
	}
	
	  Códigos da classe “Produtos”:

import javax swing JOptionPane;
public class Produtos {

double torneira,chuveiro,minutos,litros;
int descarga;
int a= 0;
String minutostring ="";

	 

public double Minutos(){// calculando minutos gastos.

Excecao ex = new Excecao();// instancia

double minutos = 0;

JOptionPane showMessage Dialog(null, "Digite a quantidade de minutos que
você utza diariamente este produto” ,
“Minutos”, JOptionPane.INFORMATION MESSAGE);
while(a==0) {
minutostring = JOptionPane.showinpulDialog("Minutos:")
a=ex.tratarmin(minutostring);
}

	 minutos = Double.parseDouble(minutostring);
	 
this.minutos=minutos;
return minutos;
}
public int Descarga() { // método que administra o calculo da descarga
int descarga=0;
JOptionPane.showMessageDialog(null,"Digite a quantidade de vezes que é acionado a descarga por dia",
	"Descarga", JOptionPane.INFORMATION_MESSAGE);	

descarga = Integer.parsein(JOpionPane.showInputDialog ("Descarga:"));


this.descarga = descarga;
return descarga;
}
public double calLiros(double litros) (// método que calcula a quantidade de litros gastos em conta		
double valor=0;
valor= (30*(ltros/1000))*2.99;

Códigos da classe "Teste":

import javax.swing.JOptionPane;,
public class Teste {

public static void main(Stringl[] args) {
Sting opcao = "";
int opt, a=0;
Excecao ex = new Excecao());

CalculaProduto prod = new CalculaProduto(); // instanciando classe

“while(a==0){// tratamento da opção

opcao = JOptionPane.showInputDialog(null,"Olá, seja bem vindo!\n "+
“Escolha o produto que deseja analizar" +
"n 1 torneira” +
"\n 2"+
" chuveiro" +
"\n 3 descarga\n"+
“Escolha a Opção:"," Analisar gastos de
agua”,JOptionPane.INFORMATION_MESSAGE);
a=ex.tratar(opcao);
}

opt-= Integer.parselnt(opcao);
prod.CalculaProduto(opt);
JOptionPane.showMessageDialog(null, "Economize agua para o bem do nosso planeta." +
     "\n Economize no banho,"+
     "\n ao escovar os dentes" +
     "\n no momento de lavar o pratos" +
     "\n e quando for dar descarga"
     ,"Mensagem ao Usuário",
JOptionPane INFORMATION MESSAGE);
}
