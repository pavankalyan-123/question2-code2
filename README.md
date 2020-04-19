# question2-code2
round robin algorithm



int isc=0, ifc= 0, min, flag; 
 	if( fc!=0  && sc!=0){  	 	while(isc<sc && ifc<fc){  	 	if(f[ifc].arrivalTime == s[isc].arrivalTime){ 
	 	 	 	m[mc] = f[ifc]; 
 	 	 	 	mc++; 
 	 	 	 	ifc++; 
 	 	 	 	m[mc]= s[isc]; 
 	 	 	 	mc++;  	 	 	 	isc++; 
 	 	 	} 
 	 	 	else if(f[ifc].arrivalTime < s[isc].arrivalTime){ 
 	 	 	 	m[mc]= f[ifc]; 
 	 	 	 	mc++;  	 	 	 	ifc++; 
 	 	 	} 
 	 	 	else if(f[ifc].arrivalTime > s[isc].arrivalTime){ 
 	 	 	 	m[mc]= s[isc]; 
 	 	 	 	mc++;  	 	 	 	isc++; 
 	 	 	} 
 	 	 	else; 
 	 	} 
 	 	if(mc != (fc+sc)){  	 	 	if(fc!=ifc){  	 	 	 	while(ifc!=fc){  	 	 	 	 	m[mc]= f[ifc]; 
 	 	 	 	 	mc++; 
 	 	 	 	 	ifc++; 
 	 	 	 	} 
 	 	 	} 
 	 	 	else if(sc!=isc){  	 	 	 	while(isc!=sc){ 
 	 	 	 	 	m[mc]= s[isc]; 
 	 	 	 	 	mc++;  	 	 	 	 	isc++; 
 	 	 	 	} 
 	 	 	}  	 	} 
 	} 
 	else if(fc==0){ 
 	 	while(isc!=sc){ 
 	 	 	m[mc]= s[isc]; 
 	 	 	mc++;  	 	 	isc++; 
 	 	} 
 	} 
 	else if(sc==0){ 
 	 	while(ifc!=fc){ 
 	 	 	m[mc]= f[ifc]; 
 	 	 	mc++;  	 	 	ifc++; 
 	 	} 
 	} 
 	else { 
	 	printf("\n No valid Jobs available\n"); 
 	} 
} 
 
