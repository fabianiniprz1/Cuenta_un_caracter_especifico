declare @Frase				varchar(150)= 'verifica la cantidad de caracteres'
declare @Caracter_buscado	varchar(1)	= 'a'
declare @Cantidad_de_caracteres int = 0

		declare @inicial int = 1, @posicion int, @final int = len(@Frase)

		while(@inicial<@final)
		begin

			set @posicion = (charindex(@Caracter_buscado,substring(@Frase,@inicial,@final-@inicial+1)))
			
			if (@posicion > 0)
			begin

			set @inicial += @posicion
			set @Cantidad_de_caracteres += 1 
			
			end 
			
			if (@posicion = 0)
			
			begin
			set @inicial =	@final
			end

			

		end

		print ('La frase "'+@Frase+'" tiente: '+convert(varchar(2),@Cantidad_de_caracteres)+' caracteres iguales a: "'+@Caracter_buscado+'"')
