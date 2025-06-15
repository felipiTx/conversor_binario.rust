use std::io;

fn main() {
    println!("Digite um texto para converter em binário:");

    let mut entrada = String::new();
    io::stdin()
        .read_line(&mut entrada)
        .expect("Erro ao ler entrada");

    let texto = entrada.trim();

    let binario: Vec<String> = texto
        .chars()
        .map(|c| format!("{:08b}", c as u8)) // 8 bits por caractere
        .collect();

    println!("\nTexto original: {}", texto);
    println!("Binário: {}", binario.join(" "));
}
