<section class="show-area">{display}</section>

<section class="buttons-container">
	<button class="top-row-button" on:click={handleClear}>AC</button>
	<button class="top-row-button" on:click={handlePlusMinus}>
		<PlusMinus />
	</button>
	<button class="top-row-button" on:click={handlePercent}>%</button>
	<button class="operation-button" on:click={() => handleOperation('/')}>
		<Division />
	</button>
	<button class="number-button" on:click={() => handleNumber('7')}>7</button>
	<button class="number-button" on:click={() => handleNumber('8')}>8</button>
	<button class="number-button" on:click={() => handleNumber('9')}>9</button>
	<button class="operation-button" on:click={() => handleOperation('*')}>
		<Multiply />
	</button>
	<button class="number-button" on:click={() => handleNumber('4')}>4</button>
	<button class="number-button" on:click={() => handleNumber('5')}>5</button>
	<button class="number-button" on:click={() => handleNumber('6')}>6</button>
	<button class="operation-button" on:click={() => handleOperation('-')}>
		<Minus />
	</button>
	<button class="number-button" on:click={() => handleNumber('1')}>1</button>
	<button class="number-button" on:click={() => handleNumber('2')}>2</button>
	<button class="number-button" on:click={() => handleNumber('3')}>3</button>
	<button class="operation-button" on:click={() => handleOperation('+')}>
		<Plus />
	</button>
	<button class="number-button curved-bottom-left-button" on:click={() => handleNumber('0')} style:grid-column="1 / span 2">
		0
	</button>
	<button class="number-button" on:click={() => handleNumber('.')}>.</button>
	<button class="operation-button curved-bottom-right-button" on:click={evaluate}>
		<Equal />
	</button>
</section>
