# CornerNet_Lite
learn note of CornerNet_Lite

# model architecture

CornerNet_Saccade

layer_name	In_dim	Out_dim	feature_size		
Input	\	3	511*511		Backbone
Conv7-BN-ReLU	3	128	256*256		
Residual-s=2	128	256	128*128		
Residual-s=2	256	256	64*64		
hg-up(fire modules)	256	256	64*64		
hg-max(none)	256	256	64*64		
hg-low1(fire modules-s=2)	256	384	32*32		
hg-low2(3 groups hg)	384	384	16*16	att1	
hg-low3(fire modules)	256	256	32*32	att2	
hg-up2(ConvTrans)	256	256	64*64	att3	
conv	256	256	64*64	inter-sup	
inter(Residual)	256	256	64*64		
hg-up(fire modules)	256	256	64*64		
hg-max(none)	256	256	64*64		
hg-low1(fire modules-s=2)	256	384	32*32		
hg-low2(3 groups hg)	384	384	16*16	att1	
hg-low3(fire modules)	256	256	32*32	att2	
hg-up2(ConvTrans)	256	256	64*64	att3	
conv	256	256	64*64		
tl_module(corner_pool)	256	256	64*64		Det
tl_heats	256	cls	64*64	parall	
tl_tags	256	1	64*64		
tl_offs	256	2	64*64		
