# useEffect Hook
	// useEffect(() => {
		console.log("in the effect");
	}, []);
	
	1) When does it run? Before or after render?
	useEffect happens after Render. 
	With empty dependency array useEffect runs in this order and only once on initial page load:
	1.First Render (Monut) -> 2.useEffect runs -> 3.user interacts (causes render) -> 4.no more effects
	With a value passed into the dependency array
	
	2) How often does it run?
	useEffect happens after Render. With no dependency array it runs every render.
	
	3) How does the dependency array change how often it runs?




# References