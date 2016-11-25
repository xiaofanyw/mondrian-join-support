# mondrian-join-support

 this patch apply to mondrian 4.4 , support left and right join for mondrian
 you need to define join information in cube tag like this:

    <Joins>
	    <Join joinType='left' >
	        <JoinTable tableName='ADZONE'>
	            <Column name='DESCRIPTION' />
	            <Column name='NAME' />
	        </JoinTable>
	        <JoinTable tableName='AD_AREA_NEW'>
	            <Column name='COUNTRY_NAME' />
	            <Column name='PROVINCE_NAME' />
	        </JoinTable>
	    </Join>
	</Joins>

