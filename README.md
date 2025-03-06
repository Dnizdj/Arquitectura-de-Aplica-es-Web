# Arquitectura-de-Aplica-es-Web

Copie o código e rode a extensão Springboot.

Segue o código:
____________________________________________________________________________________________________________________________________________________

package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
@RestController
public class DemoApplication {

	public static void main(String[] args) {
		SpringApplication.run(DemoApplication.class, args);
	}

	@GetMapping("/hello")
	public String hello(@RequestParam(value = "name", defaultValue = "Junior") String name) {
		return String.format("Denis %s", name);
	}

}

_____________________________________________________________________________________________________________________________________________________
Segue a foto:
-----------------------------------------------------------------------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/f229f182-fe30-4ef3-96bc-4edc1992b2b1)




