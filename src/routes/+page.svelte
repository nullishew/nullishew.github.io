<script>
  $effect(() => {
		const navObserver = new IntersectionObserver(
			(entries) =>
				entries.forEach((entry) => {
					const isActive = entry.isIntersecting && entry.intersectionRatio > 0.5;
					const elem = entry.target;
					elem.classList.toggle('active', isActive);
					document
						.querySelectorAll(`[href="#${elem.getAttribute('id')}"]`)
						.forEach((elem) => elem.classList.toggle('active', isActive));
				}),
			{ threshold: 0.5 }
		);

		[...document.querySelectorAll('section')]
			.filter((elem) => elem.hasAttribute('id'))
			.forEach((elem) => navObserver.observe(elem));
	});
</script>

<header>
	<nav>
		<ul>
			<li><a href="#home">Home</a></li>
			<li><a href="#about">About</a></li>
			<li><a href="#experience">Experience</a></li>
			<li><a href="#projects">Projects</a></li>
		</ul>
	</nav>
</header>

<section class="banner" id="home">
	<div class="parallax" style="position:absolute;z-index:-1">
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax0.png"
			style="--parallax-speed: .02"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax1.png"
			style="--parallax-speed: .05"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax2.png"
			style="--parallax-speed: .11"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax3.png"
			style="--parallax-speed: .16"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax4.png"
			style="--parallax-speed: .26"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax5.png"
			style="--parallax-speed: .36"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax6.png"
			style="--parallax-speed: .49"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax7.png"
			style="--parallax-speed: .69"
		/>
		<img
			src="https://www.firewatchgame.com/images/parallax/parallax8.png"
			style="--parallax-speed: 1"
		/>
	</div>
	<h1>0%</h1>
	<h2>success rate</h2>
</section>

<main>
	<section id="about" style="background: #210002; color: #ffaf00">
		<h2>hello</h2>
		<h3>idk what to put here, so...</h3>
		<p>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates cum magnam ratione, labore
			blanditiis illo alias vel, reiciendis dolorem eius odio ut inventore, nobis amet perspiciatis
			pariatur possimus minus enim ducimus. Quod assumenda, tempora neque placeat magnam nesciunt
			voluptas vel veniam ea laboriosam, impedit pariatur facilis a nulla officiis voluptate
			perferendis? Perferendis, natus odit, nulla dolores tempore repellat illum totam obcaecati
			temporibus dolor quia sequi sint quasi, veritatis neque?<br />
			Cupiditate amet perspiciatis pariatur officia perferendis laborum, obcaecati dolorem beatae consectetur
			nostrum dignissimos minima similique, sapiente illum fugiat omnis nesciunt, expedita a eos doloremque
			vel. Exercitationem quae tempore asperiores similique, dicta, laborum sit rem corrupti magnam perferendis
			atque aspernatur, facere architecto voluptatum accusamus laboriosam optio fuga? Ex ipsa illo eos,
			laboriosam, itaque reprehenderit voluptate vitae deserunt neque et minima alias dolor aperiam amet
			consectetur deleniti aspernatur recusandae ut dolores.<br />
			Nulla hic, eos sint quod tempore maxime eaque dolores ipsa nam veritatis illo, reiciendis adipisci
			et deserunt ut dignissimos eligendi dolorem repellat aperiam. Corrupti vel at ipsum quas fugit
			pariatur voluptate libero cumque iusto, culpa eligendi fugiat voluptates ab. Quo assumenda voluptate
			dolor earum totam deserunt ab, eaque explicabo provident qui libero corporis iusto quas ad necessitatibus
			sint magni, debitis ullam! Dolor suscipit facilis eaque nesciunt nihil aliquam iusto.<br />
			Iusto hic perferendis repellendus neque facere fugit ut iure eveniet, quos consectetur quibusdam
			aspernatur voluptatem earum odit dolor quasi quo maiores iste sequi fugiat asperiores ullam, nihil
			tempora! Rem nemo veniam vero odit, unde quaerat laboriosam cumque autem tempore dolorum quos similique
			incidunt nihil accusamus voluptas cum porro impedit, qui aperiam. Quis, vitae libero, quibusdam
			magni dicta et, odit eos illum illo dolorem sint ad ullam dolore in laborum?<br />
			Qui explicabo nesciunt possimus exercitationem quia a earum fugiat? Possimus, accusantium natus
			delectus labore autem architecto eius non velit tempora quis odit in placeat nisi distinctio laudantium
			voluptatum et dicta sit, nemo expedita voluptates excepturi incidunt quas? Nisi magnam repudiandae
			tempora consequuntur aspernatur omnis, deleniti ratione sunt similique? Laborum adipisci assumenda
			quibusdam veritatis! Praesentium impedit fugit reprehenderit, quod eligendi unde, et est repudiandae,
			iusto explicabo iste illo veritatis deleniti?
		</p>
	</section>
	<section id="projects" style="background: #210002; color: #ffaf00">
		<h2>projects</h2>
		<h3>idk what to put here, so...</h3>
		<p>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates cum magnam ratione, labore
			blanditiis illo alias vel, reiciendis dolorem eius odio ut inventore, nobis amet perspiciatis
			pariatur possimus minus enim ducimus. Quod assumenda, tempora neque placeat magnam nesciunt
			voluptas vel veniam ea laboriosam, impedit pariatur facilis a nulla officiis voluptate
			perferendis? Perferendis, natus odit, nulla dolores tempore repellat illum totam obcaecati
			temporibus dolor quia sequi sint quasi, veritatis neque?<br />
			Cupiditate amet perspiciatis pariatur officia perferendis laborum, obcaecati dolorem beatae consectetur
			nostrum dignissimos minima similique, sapiente illum fugiat omnis nesciunt, expedita a eos doloremque
			vel. Exercitationem quae tempore asperiores similique, dicta, laborum sit rem corrupti magnam perferendis
			atque aspernatur, facere architecto voluptatum accusamus laboriosam optio fuga? Ex ipsa illo eos,
			laboriosam, itaque reprehenderit voluptate vitae deserunt neque et minima alias dolor aperiam amet
			consectetur deleniti aspernatur recusandae ut dolores.<br />
			Nulla hic, eos sint quod tempore maxime eaque dolores ipsa nam veritatis illo, reiciendis adipisci
			et deserunt ut dignissimos eligendi dolorem repellat aperiam. Corrupti vel at ipsum quas fugit
			pariatur voluptate libero cumque iusto, culpa eligendi fugiat voluptates ab. Quo assumenda voluptate
			dolor earum totam deserunt ab, eaque explicabo provident qui libero corporis iusto quas ad necessitatibus
			sint magni, debitis ullam! Dolor suscipit facilis eaque nesciunt nihil aliquam iusto.<br />
			Iusto hic perferendis repellendus neque facere fugit ut iure eveniet, quos consectetur quibusdam
			aspernatur voluptatem earum odit dolor quasi quo maiores iste sequi fugiat asperiores ullam, nihil
			tempora! Rem nemo veniam vero odit, unde quaerat laboriosam cumque autem tempore dolorum quos similique
			incidunt nihil accusamus voluptas cum porro impedit, qui aperiam. Quis, vitae libero, quibusdam
			magni dicta et, odit eos illum illo dolorem sint ad ullam dolore in laborum?<br />
			Qui explicabo nesciunt possimus exercitationem quia a earum fugiat? Possimus, accusantium natus
			delectus labore autem architecto eius non velit tempora quis odit in placeat nisi distinctio laudantium
			voluptatum et dicta sit, nemo expedita voluptates excepturi incidunt quas? Nisi magnam repudiandae
			tempora consequuntur aspernatur omnis, deleniti ratione sunt similique? Laborum adipisci assumenda
			quibusdam veritatis! Praesentium impedit fugit reprehenderit, quod eligendi unde, et est repudiandae,
			iusto explicabo iste illo veritatis deleniti?
		</p>
	</section>
	<section id="experience" style="background: #210002; color: #ffaf00">
		<h2>experience</h2>
		<h3>idk what to put here, so...</h3>
		<p>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates cum magnam ratione, labore
			blanditiis illo alias vel, reiciendis dolorem eius odio ut inventore, nobis amet perspiciatis
			pariatur possimus minus enim ducimus. Quod assumenda, tempora neque placeat magnam nesciunt
			voluptas vel veniam ea laboriosam, impedit pariatur facilis a nulla officiis voluptate
			perferendis? Perferendis, natus odit, nulla dolores tempore repellat illum totam obcaecati
			temporibus dolor quia sequi sint quasi, veritatis neque?<br />
			Cupiditate amet perspiciatis pariatur officia perferendis laborum, obcaecati dolorem beatae consectetur
			nostrum dignissimos minima similique, sapiente illum fugiat omnis nesciunt, expedita a eos doloremque
			vel. Exercitationem quae tempore asperiores similique, dicta, laborum sit rem corrupti magnam perferendis
			atque aspernatur, facere architecto voluptatum accusamus laboriosam optio fuga? Ex ipsa illo eos,
			laboriosam, itaque reprehenderit voluptate vitae deserunt neque et minima alias dolor aperiam amet
			consectetur deleniti aspernatur recusandae ut dolores.<br />
			Nulla hic, eos sint quod tempore maxime eaque dolores ipsa nam veritatis illo, reiciendis adipisci
			et deserunt ut dignissimos eligendi dolorem repellat aperiam. Corrupti vel at ipsum quas fugit
			pariatur voluptate libero cumque iusto, culpa eligendi fugiat voluptates ab. Quo assumenda voluptate
			dolor earum totam deserunt ab, eaque explicabo provident qui libero corporis iusto quas ad necessitatibus
			sint magni, debitis ullam! Dolor suscipit facilis eaque nesciunt nihil aliquam iusto.<br />
			Iusto hic perferendis repellendus neque facere fugit ut iure eveniet, quos consectetur quibusdam
			aspernatur voluptatem earum odit dolor quasi quo maiores iste sequi fugiat asperiores ullam, nihil
			tempora! Rem nemo veniam vero odit, unde quaerat laboriosam cumque autem tempore dolorum quos similique
			incidunt nihil accusamus voluptas cum porro impedit, qui aperiam. Quis, vitae libero, quibusdam
			magni dicta et, odit eos illum illo dolorem sint ad ullam dolore in laborum?<br />
			Qui explicabo nesciunt possimus exercitationem quia a earum fugiat? Possimus, accusantium natus
			delectus labore autem architecto eius non velit tempora quis odit in placeat nisi distinctio laudantium
			voluptatum et dicta sit, nemo expedita voluptates excepturi incidunt quas? Nisi magnam repudiandae
			tempora consequuntur aspernatur omnis, deleniti ratione sunt similique? Laborum adipisci assumenda
			quibusdam veritatis! Praesentium impedit fugit reprehenderit, quod eligendi unde, et est repudiandae,
			iusto explicabo iste illo veritatis deleniti?
		</p>
	</section>
</main>

<style>
</style>
